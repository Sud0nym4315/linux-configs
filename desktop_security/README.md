Linux PC preventative/detective control scripts

Prerequisites:
- ntfy server
- web server
- Hosts connected via SDN (e.g ZeroTier)

Process:
1) script executes upon login. 
2) Fswebcam takes front-facing picture
3) PC sends webcam capture to HTTP server over SSH
4) PC then sends HTTP post request to ntfy server with a link to the image
