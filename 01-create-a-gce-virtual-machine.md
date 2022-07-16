# Create a GCE virtual machine
First, you need login to your [google cloud account](https://console.cloud.google.com) and select the project in which you want to create your vpn server, then in the right side bar menu search google compute engine and select [VM instances](https://console.cloud.google.com/compute/instances).
Click on the button [CREATE INSTANCE](https://console.cloud.google.com/compute/instancesAdd) at the top
![](images/gce-create-instance.PNG)
We will create an Ubuntu 20.04 LTS vm,
we fill the fields as follow
Name: pritunl-vpn-server<br>
region: europe-west1<br>
Machine family<br>
serie: N1<br>
![](images/pritunl-server-creation.PNG)<br>
Boot disk<br>
image: Ubuntu 20.04 LTS<br>
Firewall<br>
coche the two cases (ALLOW HTTP traffic and ALLOW HTTPS traffic)<br>
![](images/pritunl-server-creation-1.PNG)<br>
Expand the Networking section and coche enable under IP forwarding<br>
![](images/enable-ip-forwarding.PNG)<br>
And leave all others fields with default value, then click create.<br>
Alright, we have our virtual machine on GCP, let's go and [install pritunl](https://github.com/Donutson/VPN-SERVER-PRITUNL/blob/main/02-install-pritunl.md) on it.
