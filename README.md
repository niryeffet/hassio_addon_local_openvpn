# Openvpn

This is a minimalistic Homeassistant local add-on to run openvpn(s) on your network.

Installation:
* In Homeassistant, using ssh terminal clone to /addons.
* Go to Settings -> Add-ons -> ADD-ON STORE -> three dots on the top -> Check for updates
* Refresh the page, you should see Openvpn under Local Add-ons.
* Click on it, click install.

Configuration:
* See the `/example` directory.
* Start the addon. Do not worry about the warnings in the addon log.
* Using ssh, run `docker exec -it addon_local_openvpn bash -l`.
* Place your openvpn configuration files in `/data/openvpn`.
* Create your first openvpn service using `mkdir -p /data/services.d/openvpn1`.
* In the `/data/services.d/openvpn1` directory place the `run` file - see example.
* Using Homeassistant settings, restart the addon. Check the log.
