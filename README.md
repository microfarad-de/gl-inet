# GL.iNet GL-X750 "Spitz" Toolbox

Scripts for enhancing the GL.iNet GL-X750 "Spitz" (and similar GL.iNet routers) wireless router functionality.

The following scripts are available:

* [`clients`](https://github.com/microfarad-de/gl-inet/blob/main/clients): Prints a lists of connected Wi-Fi clients.

* [`speedtest`](https://github.com/microfarad-de/gl-inet/blob/main/speedtest): Performs an internet connection speed test. Depends on the `speedtest-netperf` package.

* [`modem_reset`](https://github.com/microfarad-de/gl-inet/blob/main/modem_reset): Performs modem hard reset by turning off and on the PCI power.

* [`wireguard_watchdog_khr`](https://github.com/microfarad-de/gl-inet/blob/main/wireguard_watchdog_khr): Enables stable operation with a Wireguard server behind dynamic DNS. Monitors the internet connection and automatically restarts the Wireguard service upon server IP address update. This script is not required for firmware version 4.0 which seems to automatically resolve the updated IP address.

* [`system_watchdog_khr`](https://github.com/microfarad-de/gl-inet/blob/main/system_watchdog_khr): Monitors the internet connection by periodically pinging the DNS server. A modem hard reset is performed upon repeated connectivity loss. If the connectivity loss persits following a modem reset, the script performs a modem reboot.

