# Cloudflare Trace API
Get IP Address, TimeStamp, User Agent, Country Code, IATA, HTTP Version, TLS/SSL Version &amp; more by Cloudflare

#### Endpoints:
https://one.one.one.one/cdn-cgi/trace <br>
https://1.0.0.1/cdn-cgi/trace <br>
https://cloudflare-dns.com/cdn-cgi/trace <br>
https://cloudflare-eth.com/cdn-cgi/trace <br>
https://workers.dev/cdn-cgi/trace <br>
https://pages.dev/cdn-cgi/trace <br>
https://cloudflare.tv/cdn-cgi/trace <br>
https://icanhazip.com/cdn-cgi/trace <br>

#### Return Format:
<pre>
fl=Cloudflare WebServer Instance
h=WebServer <a href="https://en.wikipedia.org/wiki/Hostname">Hostname</a>
ip=IP Address of client
ts=<a href="https://en.wikipedia.org/wiki/Unix_time">Epoch Time</a> in seconds.millis (Similar to `date +%s.%3N` in bash)
visit_scheme=https or http
uag=<a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/User-Agent">User Agent</a>
colo=<a href="https://en.wikipedia.org/wiki/IATA_airport_code">IATA location identifier</a>
sliver=Whether the request is splitted
http=<a href="https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol">HTTP Version</a>
loc=<a href="https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2">Country Code</a>
tls=<a href="https://en.wikipedia.org/wiki/Transport_Layer_Security">TLS</a> or SSL Version
sni=Whether <a href="https://en.wikipedia.org/wiki/Server_Name_Indication">SNI</a> encrypted or plaintext
warp=Whether client over <a href="https://1.1.1.1/">Cloudflares Wireguard VPN</a>
gateway=Whether client over <a href="https://www.cloudflare.com/teams/gateway/">Cloudflare Gateway</a>
rbi=Whether client over <a href="https://www.cloudflare.com/learning/access-management/what-is-browser-isolation/">Cloudflares Remote Browser Isolation</a>
kex=<a href="https://en.wikipedia.org/wiki/Key_exchange">Key exchange</a> method for TLS
</pre>

## Cloudflare Geolocation API

#### Endpoint:
https://speed.cloudflare.com/meta

#### Return Format:
```json
{
  "hostname": "speed.cloudflare.com",
  "clientIp": "69.193.168.152",
  "httpProtocol": "HTTP/1.1",
  "asn": 13254,
  "asOrganization": "My Organisation",
  "colo": "JFK",
  "country": "US",
  "city": "New York City",
  "region": "New York",
  "postalCode": "10001",
  "latitude": "40.730610",
  "longitude": "-73.935242"
}
```

#### Endpoint:
https://speed.cloudflare.com/__down  

#### Return Data In Headers:
```json
{
  "cf-meta-asn": "13254",
  "cf-meta-city": "New York City",
  "cf-meta-colo": "JFK",
  "cf-meta-country": "US",
  "cf-meta-ip": "69.193.168.152",
  "cf-meta-latitude": "40.730610",
  "cf-meta-longitude": "-73.935242",
  "cf-meta-postalcode": "10001",
  "cf-meta-request-time": "1724183717263",
  "cf-meta-timezone": "America/New_York"
}

```

#### Other Resources:
[Convert Return Format to JSON](https://stackoverflow.com/a/68304489/2437224)

[IATA List](https://cdn.jsdelivr.net/gh/fawazahmed0/iata-list@main/iata.json)

#### Other Useful Endpoints by cloudflare:


[DNS Over HTTPS API](https://developers.cloudflare.com/1.1.1.1/encryption/dns-over-https/make-api-requests/dns-json)
