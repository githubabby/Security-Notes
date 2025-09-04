protocols

FTP - file transfer protocol
if you are sending things that should not be publically accessible like your code or files with passwords and keys.. they are clear text which others can see.
using it is bad.

SFTP-secure file transfer protocol.

Telnet - control one computer from another. connect to remote computer. could use to connect to appliances.
Now we use SSH - encrpt the trafic

HTTP - sent in the clear, like a session - more like sessionid. header or cookie.
lack of encrpytion. can have anything sensitive like creds, card info or data you give in forms.

MySQL itself is not encrpted, so keep it on same network, even if it is on different server so information is in the same network and not leaving out.

Never run a webserver as root/administrator priviledge. that's hy we run them as appache or httpd.