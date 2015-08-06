# type: socket

These inspectors expose the sockets opened on the network on the endpoint.

# local address of &lt;socket&gt; : ipv4or6 address

Returns the local address of the socket.

{% qna %}
Q: unique values of local addresses of sockets of network
A: 0.0.0.0
A: 10.0.2.15
A: 127.0.0.1
A: 0:0:0:0:0:0:0:0
A: 0:0:0:0:0:0:0:1
A: fe80:0:0:0:3422:3b00:e7f8:c486
A: fe80:0:0:0:3c5b:1dd4:2963:510e
{% endqna %}

# local port of &lt;socket&gt; : integer

Returns the local port number of the socket.

{% qna %}
Q: unique values of local ports of sockets of network
A: 135
A: 137
A: 138
A: 139
A: 445
A: 546
{% endqna %}

# process of &lt;socket&gt; : process

Returns the process that owns the socket.

{% qna %}
Q: unique values of names of processes of sockets of network
A: System
A: chrome.exe
A: javaw.exe
{% endqna %}

# remote address of &lt;socket&gt; : ipv4or6 address

Returns the remote address of the socket.

{% qna %}
Q: unique values of remote addresses of sockets of network
A: 74.125.25.103
A: 127.0.0.1
{% endqna %}

# remote port of &lt;socket&gt; : integer

Returns the remote port number of the socket.

{% qna %}
Q: unique values of remote ports of sockets of network
A: 443
A: 49707
A: 49708
{% endqna %}

# tcp of &lt;socket&gt; : boolean

Returns `True` if the socket is a TCP socket.

{% qna %}
Q: unique values of remote ports of sockets whose (tcp of it) of network
A: 80
A: 443
A: 49707
A: 49708
{% endqna %}

# tcp state of &lt;socket&gt; : tcp state

Returns the tcp state of the socket.

{% qna %}
Q: (remote ports of it, tcp states of it) of sockets whose (tcp of it) of network
A: 443, TIME_WAIT
A: 80, TIME_WAIT
A: 443, ESTABLISHED
A: 49708, ESTABLISHED
A: 49707, ESTABLISHED
{% endqna %}

# udp of &lt;socket&gt; : boolean

Returns `True` if the socket is a UDP socket.

{% qna %}
Q: exists socket whose (udp of it) of network
A: True
{% endqna %}
