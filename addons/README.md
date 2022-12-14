# Addons

HA OS supports various addons that allow the user to extend the functionality around Home Assistant 
by installing additional applications. More info can be found at the [Home Assistant Add-ons](https://www.home-assistant.io/addons/) page.

Here is a list of the add ons that I have used in the past (or currently using) and find pretty useful:

### Mosquito broker

The Mosquitto project runs a public MQTT broker. MQTT (aka MQ Telemetry Transport) is a machine-to-machine or  “Internet of Things” connectivity protocol on top of TCP/IP. It allows extremely lightweight publish/subscribe  messaging transport. MQTT provides an easy and robust way of transferring data (information & commands) between various devices and HA.

### DuckDNS

The DuckDNS integration allows you to keep your DuckDNS subdomain always in sync with your public IP address. DuckDNS is a free service that allows you to bind your own favorite subdomain under duckdns.org to the public IP address in use from your router, even though such address is dynamically allocated by your internet service provider and therefore changes over time.

### Terminal

This add-on allows you to log in to your Home Assistant instance using SSH or a Web Terminal, giving you to access your folders and also includes a command-line tool to do things like restart, update, and check your instance.

### Studio Code Server

This add-on runs Visual Studio Code, allowing you to edit your Home Assistant configuration straight from the web browser and can be embedded straight into the Home Assistant frontend UI. Visual Studio Code runs as a remote server using code-server, and is a fully-fledged VSCode experience.

### AdGuard Home

AdGuard Home is a network-wide ad- and tracker-blocking DNS server with parental control (adult content blocking) capabilities. The AdGuard integration allows you to control and monitor your AdGuard Home instance in Home Assistant.
