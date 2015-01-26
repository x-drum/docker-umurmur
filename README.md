# docker-umurmur
# Simple container for uMurmur (a minimalistic Mumble server)

## Usage
Assuming that your SSL certificates are under "/path/to/sslcerts" and matching your umurmur.conf:

```bash
docker run -ti --rm -p 64738:64738/udp -p 64738:64738 -v /path/to/umurmur.conf:/etc/umurmur.conf -v /path/to/sslcerts:/etc/umurmur xdrum/umurmur 
```
