# webrtc-sip
webrtc jssip prototype

Must add SIP server configuration at _index.js_ before testing.
```
var configuration = {
    'uri': 'sip:user@domain',
    'password': '', // FILL PASSWORD HERE,
    'ws_servers': 'wss://<ws server ip or fqdn>:<port>/'
};
```
# supported use cases
__It's only tested on Chrome__ on CentOS

1. Outbound/Inbound call to a North American DID
2. Outbound/Inbound call to an extention
3. Video call to Monster UI WebRTC
4. Conference call

## Known bugs
1. If the remote terminates an outbound call, JsSIP will not trigger the right callback. But this seems 
FS issue.

JsSIP:Transport received WebSocket text message:
SIP/2.0 486 Unable to Comply

https://groups.google.com/forum/#!topic/2600hz-dev/krikOmTA61E

