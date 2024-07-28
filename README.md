# Listen
On one computer listen to events on some port via `nc` command
Run `nc -l 1234`

# Send
On other computer seelct file to send and transmit it via
`cat test | nc 192.168.31.66 1234`

# Sending multiple files
We can zip those files and send them via network
`tar cf - . | nc 192.168.31.66 1234`
On the other side save changes to file like `received.tar`