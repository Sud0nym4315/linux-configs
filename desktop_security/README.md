The "detect" script needs the followng things to run as I have it:

- A sudoer's entry that allows a non-root user to execute without a password
- A web server to send login captures to
- A ntfy server to send notifications to subscribed devices


The script takes a front-facing webcam picture, sends it over SSH to a web server to host the image, and sends a POST request to an "ntfy" server with the link to the webcam capture.
