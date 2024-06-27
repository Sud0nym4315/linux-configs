The "detect" script needs the following things to run as I have it:

- A sudoer's entry that allows a non-root user to execute without a password
- A web server to send login captures to via SSH
- A ntfy server to send notifications to subscribed devices


The script takes a front-facing webcam picture, sends it over SSH to a web server to host the image, and sends a POST request to an "ntfy" server with the link to the webcam capture. A phone subscribed to the appropriate ntfy channel and server will receive the login details and picture
