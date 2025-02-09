# Zabbix template for BIRD2.0

This is a Zabbix template for monitoring BIRD 2.0 routing daemon with [birdwatcher](https://github.com/alice-lg/birdwatcher).

## Usage

1. Import the template [`bird2.0-by-http.yaml`](bird2.0-by-http.yaml) into your Zabbix.
2. Make sure that [`birdwatcher`](https://github.com/alice-lg/birdwatcher) is running on your router and accessible from the Zabbix server.
3. Add the following Macros to the host:
   - `{$BIRDWATCHER.URL.HOST}` - IP address or hostname of the router with BIRD
   - `{$BIRDWATCHER.URL.PORT}` - (optional) port on which `birdwatcher` is running (default is 29184)
