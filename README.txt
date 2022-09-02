CS 558: Computer Systems Lab
Assignment–2: Socket Programming
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Submitted by:
Dhruvilkumar Megha  (214101028)
Mayank Singh Parmar (214101027)
Kumar Sandip Roy    (214101026)
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Application #4:
Multi-stage DNS Resolving System using Client-Server socket programming

Steps to run the program

1. Compile and run all the 3 program files by command:
	g++ dns.cpp -o dns
	g++ proxy.cpp -o proxy
	g++ client.cpp -o client

2. Open new terminal in same directory and write command:
	./dns 8000
	(here 8000 is the dns port number and can be replaced with other port number also)

3. Open another new terminal in same directory and write command:
	./proxy 9000 127.0.0.1 8000
	(9000: port number of proxy, 127.0.0.1: Loopback address(IP address), 8000: port number of DNS server)

4. Open another new terminal in same directory and write command:
	./client 127.0.0.1 9000
	(9000: port number of the proxy server)

5. To run multiple clients, open new terminal for each client and run above command.

6. Select the options:
	(1) For domain name to ip conversion
	(2) For IP to domain name conversion


NOTE: The database.txt file is read by DNS server and is updated by system admin
	  The cache.txt file is updated by the Proxy server and it's size can changed by programmer.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


