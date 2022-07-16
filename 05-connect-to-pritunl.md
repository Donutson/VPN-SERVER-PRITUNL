# Connection to pritunl vpn

First you need to install the pritunl client, follow the documentation [here](https://client.pritunl.com/) depending of your operating system
Now go to pritunl vpn web page (open your pritunl server ip on a browser), and next to your created Test user you will see a link symbol, click on it<br>
![](images/pritunl-user-links.PNG)<br>
Copy the last link (Temporary uri link for Pritunl Client, expires after 24 hours)<br>
![](images/pritunl-profil-link.PNG)<br>
Now open your pritunl client and click on Import Profile URI and paste in the link and click on import.<br>
![](images/pritunl-client-import-profile.PNG)<br>
The Test user profile will be display, click on the burger menu and then on the connect button, your pin will be ask, enter it and you will be connected.<br>
![](images/pritunl-connect.PNG)<br>
If you have configure your pritunl vpn to use two factor authenticator, you can use the [Authenticator addons](https://addons.mozilla.org/fr/firefox/addon/auth-helper/) to get your OTP code (i will not talk about this)
Congratulations, you are now connected to your vpn<br>
![](images/pritunl-connected.PNG)<br>
To disconnect, just click the burger menu then disconnect
