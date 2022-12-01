CFLAGS=-o
CC=gcc

all : tcpclient tcpserver udpclient udpserver

tcpclient : 
	$(CC) $(CFLAGS) tcpclient tcpclient.c -D BUFSIZE=1024 -D SADDR='struct sockaddr' -D SIZE='sizeof(struct sockaddr_in)'

tcpserver : 
	$(CC) $(CFLAGS) tcpserver tcpserver.c -D SERV_PORT=10050 -D BUFSIZE=100 -D SADDR='struct sockaddr' 
  
udpclient : 
	$(CC) $(CFLAGS) udpclient udpclient.c -D SERV_PORT=20001 -D BUFSIZE=1024 -D SADDR='struct sockaddr' -D SLEN='sizeof(struct sockaddr_in)'

udpserver : 
	$(CC) $(CFLAGS) udpserver udpserver.c -D SERV_PORT=20001 -D BUFSIZE=1024 -D SADDR='struct sockaddr' -D SLEN='sizeof(struct sockaddr_in)'
