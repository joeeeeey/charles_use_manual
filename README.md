This project is a guide to install charles and use it([crack it](https://github.com/8enet/Charles-Crack)).


## Getting started
### Set Up(MacOS)

1. Download [charles 4.2.5](https://www.charlesproxy.com/assets/release/4.2.5/charles-proxy-4.2.5.dmg).  Double click charles-proxy-xx.dmg and install it.
2. Open the application and close it.
3. Open Terminal.
4. Switch to top level directory and run `cd /Applications/Charles.app/Contents/Java/`.
5. run `open .`.
6. replace the charles.jar in by charles.jar from this repo.
7. Open charles again.
8. Install https crt.

![alt text](https://raw.githubusercontent.com/joeeeeey/charles_use_manual/master/screenshot/charles_certicate_install.png)

9. Enable charles crt.

![alt text](https://raw.githubusercontent.com/joeeeeey/charles_use_manual/master/screenshot/enable_charles_proxy_crt.png)

10. Enable charles ssl proxy
Click the topbar of charles: Proxy => SSL PROXYING => Enable SSL.
Add a list, eg: 
    HOST: xxxx.com 
    PORT: 443

11. Activate charles for macos 

![alt text](https://raw.githubusercontent.com/joeeeeey/charles_use_manual/master/screenshot/charles_enable_macos_system.png)

### Enable Proxy(System Config)
#### Only use for Chrome 
Install chrome plugin [SwitchyOmega](https://chrome.google.com/webstore/detail/proxy-switchyomega/padekgcemlokbadohgkifijomclgjgif) and config it as the following picture. Open this config.

![alt text](https://raw.githubusercontent.com/joeeeeey/charles_use_manual/master/screenshot/charles_switch_omega_config.png)


### Global use(will proxy all the http and https requests from your PC)

1. Go into Setting => Network => Advanced => Proxy
2. Both change web proxy and secure web proxy as 127.0.0.1 : 8888

![alt text](https://raw.githubusercontent.com/joeeeeey/charles_use_manual/master/screenshot/macos_network_proxy_config_for_charles.png)

### Set https proxy in iOS device

* In charles > Helper > SSL Proxying > Install certificate in mobile device.
* Set your iOS device to use Charles as its HTTP proxy in the Settings app > Wifi settings.
* Open Safari and browse to https://chls.pro/ssl. Safari will prompt you to install the SSL certificate.
* If you are on iOS 10.3 or later, open the Settings.app and navigate to General > About > Certificate Trust Settings, and find the Charles Proxy certificate, and switch it on to enable full trust for it (More information about this change in iOS 10).
* Now you should be able to access SSL websites with Charles using SSL Proxying.
Charles supports App Transport Security (ATS) as of the 3.11.4 release.

