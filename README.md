# Plex Apache Reverse Proxy
 
This configuration will allow you to serve Plex via Apache.
 
## Minimal Requirements
 
Apache
 
Plex:
* Remote Access - Disable
* Network - Custom server access URLs = `https://<your-domain>:443,http://<your-domain>:80`
* Network - Secure connections = Preferred.
* ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) `Note you can force SSL by setting required and not adding the HTTP URL, however some players which do not support HTTPS (e.g: Roku, Playstations, some SmartTVs) will no longer function.`
 
## Based on [a link](https://github.com/toomuchio/plex-nginx-reverseproxy)
 
UFW or other firewall:
* Note adding `allowLocalhostOnly="1"` to your Preferences.xml, will make Plex only listen on the localhost, achieving the same thing as using a firewall.

