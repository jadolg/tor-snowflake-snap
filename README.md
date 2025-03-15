# tor-snowflake-snap

## Installation

`snap install tor-snowflake`

## Logs

Regular snap logs are easy to check using `snap logs tor-snowflake.snowflake -f`
We also log more detailed events to a log file you can tail with `tail -f /var/snap/tor-snowflake/current/snowflake.log`

## Firewall

Make sure to open ports 32768 to 60999 UDP to be able to help more people.
* **iptables**: `sudo iptables -A INPUT -p udp --dport 32768:60999 -j ACCEPT`
* **ufw**: `sudo ufw allow 32768:60999/udp`