# Create firewall rules

In your gcp console menu bar, search network vpc and then [firewall](https://console.cloud.google.com/networking/firewalls), click on CREATE FIREWALL RULE<br>
![](images/create-firewall.PNG)<br>
We will start with the ingress rule, so use the following parameters<br>
Name: pritunl-ingress<br>
Direction of traffic: coche Ingress<br>
Target tags: pritunl-vpn (we will later tag our pritunl vm with the same tag for him to be affect by our firewall rule)<br>
Source IPV4 ranges: 0.0.0.0/0<br>
Specified protocols and ports: coche UDP and enter 10107 as value (or the port you have specified in the configuration of your pritunl instance)<br>
![](images/pritunl-ingress.PNG)
![](images/create-firewall-1.PNG)<br>
Repeat the same process to create an egress rule (just change Direction of traffic for Egress). Let's see [how to connect to our vpn](05-connect-to-pritunl.md).
