# EC601
 Cybersecurity WEBRTC
## Review
WebRTC stands for web Real-Time Communication which is a free and open-sourced project provides mobile and web a peer-to-peer communication without any plugins.
Now, WebRTC has been used in many applications, such as Google Handouts, Facebook messager, and Snapchat.

## Security
### advantages
  - No need for additional installations
  - Media access only after permission
  - Camera, microphone, screen sharing
  - Encryption on most channels : For example, SRTP over data channel
  - Fast and Automatic updated: as part of the web browser
### risks
  - IP address leak
  - Man-in-the-middle attack
  - Untrusted browsers
  
## How to fix security issues
WebRTC is mainly about three APIs: getUserMedia(), RTCPeerConnection and RTCDataChannel.

  From the view of cybersecurity, MediaDevices.getUserMedia() may be an dangerous part of user privacy. And there are several features that helps keep this method  safe.

1. getUserMedia() can only be used in secure contexts like HTPPS pages or localhost pages;

2. Only by receiving user permission could getUserMedia() get access to user's audio and video input;

3. Browsers should always display an indicator if user's camera or microphone is in use, and another indicator showing if the permission of using such input device is granted;

In normal cases, these three rules shall keep this method under control.

According to three components of WebRTC, if we want to investigate security issues in WebRTC, we should do further research in these three parts.  


# start localhost peerjs server

peerjs --port 3001

# auto deploy server

npm run devStart

# start video chat

1) go to url: localhost:5000 (https://webrtc-talk.herokuapp.com/ in construction)

2) copy the url in your current browser to another

3) bingo!
