# AmneziaWG Packages for offical GL.iNET MT-3000 router firmware

Official op24 GL.iNET firmware could be downloaded [here](https://dl.gl-inet.com/router/mt3000/open)

Installation instructions (in Russian) coud be found [here](https://github.com/openwrt-xiaomi/awg-openwrt/wiki/AmneziaWG-installing#%D1%83%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%BA%D0%B0-amneziawg-%D0%BD%D0%B0-openwrt-%D1%83%D1%81%D1%82%D1%80%D0%BE%D0%B9%D1%81%D1%82%D0%B2%D0%B5)

NOTE: in case you need to pass all traffic through AWG interface, check "Route Allowed IPs" checkbox in the Peer settings (this is absent in instruction above)

# Usage

You will have to configure Amnezia using LUCI web interface, but once configured and installed, you can continue using full power on GL.iNET interface (including VPN settings). In case your AWG interface is ON and no VPN configured in GL's UI all traffic is going through AWG, once you turn your Wireguard connection ON (in GL UI) all traffic will go through Wireguard connection (no matter about AWG status), so basically it will work like independed VPN connection with lower priority than GL.iNET's VPN.
