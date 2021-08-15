# Cloudflare Trace API
Get IP Address, TimeStamp, User Agent, Country Code, IATA, HTTP Version, TLS/SSL Version &amp; more by Cloudflare

#### Endpoint:
https://1.1.1.1/cdn-cgi/trace

#### Return Format:
<pre>
fl=Cloudflare WebServer Instance
h=WebServer <a href="https://en.wikipedia.org/wiki/Hostname">Hostname</a>
ip=IP Address of client
ts=<a href="https://en.wikipedia.org/wiki/Unix_time">Epoch Time</a> in seconds.millis (Similar to `date +%s.%3N` in bash)
visit_scheme=https or http
uag=<a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/User-Agent">User Agent</a>
colo=<a href="https://en.wikipedia.org/wiki/IATA_airport_code">IATA location identifier</a>
http=<a href="https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol">HTTP Version</a>
loc=<a href="https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2">Country Code</a>
tls=<a href="https://en.wikipedia.org/wiki/Transport_Layer_Security">TLS</a> or SSL Version
sni=Whether <a href="https://en.wikipedia.org/wiki/Server_Name_Indication">SNI</a> encrypted or plaintext
warp=Whether client over <a href="https://1.1.1.1/">Cloudflares Wireguard VPN</a>
gateway=Whether client over <a href="https://www.cloudflare.com/teams/gateway/">Cloudflare Gateway</a>
</pre>

#### Other Resources:
[Convert Return Format to JSON](https://stackoverflow.com/a/68304489/2437224)
