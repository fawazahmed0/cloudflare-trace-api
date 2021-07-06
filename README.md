# Cloudflare Trace API
Get IP Address, TimeStamp, User Agent, Country Code, IATA, HTTP Version, TLS/SSL Version &amp; More by Cloudflare

#### Endpoint:
https://cloudflare.com/cdn-cgi/trace

#### Return Format:
> fl=[Cloudflare WebServer Instance](https://community.cloudflare.com/t/what-does-the-fl-field-in-cdn-cgi-trace-represent/150595)<br>
h=WebServer [Hostname](https://en.wikipedia.org/wiki/Hostname)<br>
ip=IP Address of client<br>
ts=[Epoch Time](https://en.wikipedia.org/wiki/Unix_time) in seconds.millis (`date +%s.%3N`)<br>
visit_scheme=https or http<br>
uag=[User Agent](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/User-Agent)<br>
colo=[IATA location identifier](https://en.wikipedia.org/wiki/IATA_airport_code)<br>
http=[HTTP Version](https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol)<br>
loc=[Country Code](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)<br>
tls=[TLS](https://en.wikipedia.org/wiki/Transport_Layer_Security) or SSL Version<br>
sni=Whether [SNI](https://en.wikipedia.org/wiki/Server_Name_Indication) encrypted or plaintext<br>
warp=Whether over [Cloudflares Wireguard VPN](https://1.1.1.1/)<br>
gateway=Whether over [Cloudflare Gateway](https://www.cloudflare.com/teams/gateway/)<br>


