This project is a guide to install charles and use it([crack it](https://github.com/8enet/Charles-Crack)).


## Getting started
### Set Up(MacOS)

1. Download [charles 4.2.5](https://www.charlesproxy.com/assets/release/4.2.5/charles-proxy-4.2.5.dmg).  Double click charles-proxy-xx.dmg and install it 
2. Open the application and close it 
3. Open Terminal
4. Switch to top level directory and run `cd /Applications/Charles.app/Contents/Java/`
5. run `open .`
6. replace the charles.jar in by charles.jar from this repo
7. Open charles again.
8. Install https crt(see screenshoot/charles_certicate_install.png) 
9. Enable charles crt(see screenshoot/enable_charles_proxy_crt.png) 
10. Activate charles for macos (see screenshoot/charles_enable_macos_system)


### Enable Proxy(System Config)
#### Only use for Chrome 
Install chrome plugin [SwitchyOmega](https://chrome.google.com/webstore/detail/proxy-switchyomega/padekgcemlokbadohgkifijomclgjgif) and config it as the following picture. Open this config.

see screenshoot/charles_switch_omega_config


### Global use(will proxy all the http and https requests from your PC)

1. Go into Setting => Network => Advanced => Proxy
2. Both change web proxy and secure web proxy as 127.0.0.1 : 8888

see screenshoot/macos_network_proxy_config_for_charles
<!-- ![alt text](https://raw.githubusercontent.com/joeeeeey/simple_proxy/master/app/assets/images/mac_network_proxy_config.png) -->
