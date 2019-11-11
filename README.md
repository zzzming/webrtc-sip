# webrtc-sip
webrtc jssip prototype

Must add SIP server configuration at index.html before testing.

var configuration = {
    'uri': 'sip:user@domain',
    'password': '', // FILL PASSWORD HERE,
    'ws_servers': 'wss://<ws server ip or fqdn>:<port>/'
};

# supported use cases
__It's only tested on Chrome__

1. Outbound/Inbound call to a North American DID
2. Outbound/Inbound call to an extention
3. Video call to another JsSIP device (WebRTC) 
4. Conference call
