# Between VLAN
-----------------------------------------------------------

PC26 (RnD) to Server
```
C:\>ping 223.4.0.98

Pinging 223.4.0.98 with 32 bytes of data:

Reply from 223.4.0.98: bytes=32 time<1ms TTL=127
Reply from 223.4.0.98: bytes=32 time<1ms TTL=127
Reply from 223.4.0.98: bytes=32 time<1ms TTL=127
Reply from 223.4.0.98: bytes=32 time<1ms TTL=127

Ping statistics for 223.4.0.98:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 0ms, Maximum = 0ms, Average = 0ms

C:\>!
```

----------------------------------------------------------
PC63 (SnM) to Server
```
C:\>ping 223.4.0.98

Pinging 223.4.0.98 with 32 bytes of data:

Reply from 223.4.0.98: bytes=32 time<1ms TTL=127
Reply from 223.4.0.98: bytes=32 time<1ms TTL=127
Reply from 223.4.0.98: bytes=32 time<1ms TTL=127
Reply from 223.4.0.98: bytes=32 time<1ms TTL=127

Ping statistics for 223.4.0.98:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 0ms, Maximum = 0ms, Average = 0ms

C:\>
```
----------------------------------------------------------
PC27 (RnD) to PC63 (SnM)
```
C:\>ping server

Pinging 223.4.0.98 with 32 bytes of data:

Reply from 223.4.0.98: bytes=32 time<1ms TTL=127
Reply from 223.4.0.98: bytes=32 time<1ms TTL=127
Reply from 223.4.0.98: bytes=32 time<1ms TTL=127
Reply from 223.4.0.98: bytes=32 time<1ms TTL=127

Ping statistics for 223.4.0.98:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 0ms, Maximum = 0ms, Average = 0ms

C:\>
```
----------------------------------------------------------
PC63 (SnM) to PC26(RnD)
```
C:\>ping 223.4.0.2

Pinging 223.4.0.2 with 32 bytes of data:

Reply from 223.4.0.2: bytes=32 time<1ms TTL=127
Reply from 223.4.0.2: bytes=32 time<1ms TTL=127
Reply from 223.4.0.2: bytes=32 time<1ms TTL=127
Reply from 223.4.0.2: bytes=32 time<1ms TTL=127

Ping statistics for 223.4.0.2:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 0ms, Maximum = 0ms, Average = 0ms

C:\>
```
----------------------------------------------------------
# Demostrate access of all hosts to each and http service on the server machine
----------------------------------------------------------

PC26 (RnD) to Server
```
C:\>ping 223.4.0.98

Pinging 223.4.0.98 with 32 bytes of data:

Reply from 223.4.0.98: bytes=32 time<1ms TTL=127
Reply from 223.4.0.98: bytes=32 time<1ms TTL=127
Reply from 223.4.0.98: bytes=32 time<1ms TTL=127
Reply from 223.4.0.98: bytes=32 time<1ms TTL=127

Ping statistics for 223.4.0.98:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 0ms, Maximum = 0ms, Average = 0ms

C:\>
```
---------------------------------------------------------
PC63 (SnM) to Server
```
C:\>ping 223.4.0.98

Pinging 223.4.0.98 with 32 bytes of data:

Reply from 223.4.0.98: bytes=32 time=1ms TTL=127
Reply from 223.4.0.98: bytes=32 time<1ms TTL=127
Reply from 223.4.0.98: bytes=32 time<1ms TTL=127
Reply from 223.4.0.98: bytes=32 time=1ms TTL=127

Ping statistics for 223.4.0.98:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 0ms, Maximum = 1ms, Average = 0ms

```
---------------------------------------------------------
PC27 (RnD) to Server
```
C:\>ping 223.4.0.98

Pinging 223.4.0.98 with 32 bytes of data:

Reply from 223.4.0.98: bytes=32 time=1ms TTL=127
Reply from 223.4.0.98: bytes=32 time<1ms TTL=127
Reply from 223.4.0.98: bytes=32 time<1ms TTL=127
Reply from 223.4.0.98: bytes=32 time<1ms TTL=127

Ping statistics for 223.4.0.98:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 0ms, Maximum = 1ms, Average = 0ms

C:\>
```
-------------------------------------------------------
PC64 (SnM) to Server
```
C:\>ping 223.4.0.98

Pinging 223.4.0.98 with 32 bytes of data:

Reply from 223.4.0.98: bytes=32 time=1ms TTL=127
Reply from 223.4.0.98: bytes=32 time<1ms TTL=127
Reply from 223.4.0.98: bytes=32 time<1ms TTL=127
Reply from 223.4.0.98: bytes=32 time=1ms TTL=127

Ping statistics for 223.4.0.98:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 0ms, Maximum = 1ms, Average = 0ms

C:\>
```

-------------------------------------------------------
# Demonstrate the behavior of the internetwork when a single trunk link fails.

> Link between MainF1Switch and MainF2Switch is down
-------------------------------------------------------
PC63 to PC27 via route:
PC63 - MainF2Switch - MainF3Switch - PC27
```
C:\>ping 223.4.0.3

Pinging 223.4.0.3 with 32 bytes of data:

Reply from 223.4.0.3: bytes=32 time<1ms TTL=127
Reply from 223.4.0.3: bytes=32 time<1ms TTL=127
Reply from 223.4.0.3: bytes=32 time=5ms TTL=127
Reply from 223.4.0.3: bytes=32 time<1ms TTL=127

Ping statistics for 223.4.0.3:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 0ms, Maximum = 5ms, Average = 1ms
```

-------------------------------------------------------
PC63 to PC26 via route:
PC63 - MainF2Switch - MainF3Switch - MainF1Switch- PC26
```
C:\>ping 223.4.0.2

Pinging 223.4.0.2 with 32 bytes of data:

Reply from 223.4.0.2: bytes=32 time<1ms TTL=127
Reply from 223.4.0.2: bytes=32 time<1ms TTL=127
Reply from 223.4.0.2: bytes=32 time=6ms TTL=127
Reply from 223.4.0.2: bytes=32 time<1ms TTL=127

Ping statistics for 223.4.0.2:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 0ms, Maximum = 6ms, Average = 1ms

C:\>
```
-------------------------------------------------------
PC27 to Server via route:
PC27 - MainF3Switch - MainF1Switch - Server
```
C:\>ping 223.4.0.98

Pinging 223.4.0.98 with 32 bytes of data:

Reply from 223.4.0.98: bytes=32 time<1ms TTL=127
Reply from 223.4.0.98: bytes=32 time<1ms TTL=127
Reply from 223.4.0.98: bytes=32 time<1ms TTL=127
Reply from 223.4.0.98: bytes=32 time<1ms TTL=127

Ping statistics for 223.4.0.98:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 0ms, Maximum = 0ms, Average = 0ms

```
-------------------------------------------------------
PC64 to PC26 via route:
PC64 - MainF3Switch - MainF1Switch - PC26
```
C:\>ping 223.4.0.2

Pinging 223.4.0.2 with 32 bytes of data:

Reply from 223.4.0.2: bytes=32 time<1ms TTL=127
Reply from 223.4.0.2: bytes=32 time<1ms TTL=127
Reply from 223.4.0.2: bytes=32 time<1ms TTL=127
Reply from 223.4.0.2: bytes=32 time<1ms TTL=127

Ping statistics for 223.4.0.2:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 0ms, Maximum = 0ms, Average = 0ms

C:\>
```
-------------------------------------------------------
# DNS Demo
> Other demonstrations/tests (optional, group decision). 

> Do nslookup of "server" on dns server, Server (223.4.0.98)
-------------------------------------------------------
PC26 (RnD)
```
C:\>nslookup server 223.4.0.98

Server: [223.4.0.98]
Address:  223.4.0.98

Non-authoritative answer:
Name:   server
Address:   223.4.0.98
           
C:\>
```
-------------------------------------------------------
PC63 (SnM)
```
C:\>nslookup server 223.4.0.98

Server: [223.4.0.98]
Address:  223.4.0.98

Non-authoritative answer:
Name:   server
Address:   223.4.0.98
           
C:\>
```
-------------------------------------------------------
PC27 (RnD)
```
C:\>nslookup server 223.4.0.98

Server: [223.4.0.98]
Address:  223.4.0.98

Non-authoritative answer:
Name:   server
Address:   223.4.0.98
           
C:\>
```
--------------------------------------------------------
PC64 (SnM)
```
C:\>nslookup server 223.4.0.98

Server: [223.4.0.98]
Address:  223.4.0.98

Non-authoritative answer:
Name:   server
Address:   223.4.0.98
           
C:\>
```
--------------------------------------------------------
# Final Demostration
> Testing OSPF routing
--------------------------------------------------------
PC1 (RSales) to PC11 (admin) via:  
RSalesSwitch - RSalesRouter - MainRouter -
CentralRouter - Switch - AdminRouter - AdminSwitch 
```
C:\>ping 223.4.0.195

Pinging 223.4.0.195 with 32 bytes of data:

Request timed out.
Reply from 223.4.0.195: bytes=32 time=2ms TTL=124
Reply from 223.4.0.195: bytes=32 time=2ms TTL=124
Reply from 223.4.0.195: bytes=32 time=2ms TTL=124

Ping statistics for 223.4.0.195:
    Packets: Sent = 4, Received = 3, Lost = 1 (25% loss),
Approximate round trip times in milli-seconds:
    Minimum = 2ms, Maximum = 2ms, Average = 2ms

C:\>tracert 223.4.0.195

Tracing route to 223.4.0.195 over a maximum of 30 hops: 

  1   0 ms      0 ms      0 ms      223.4.0.113
  2   2 ms      10 ms     0 ms      223.4.0.138
  3   1 ms      2 ms      1 ms      223.4.0.142
  4   9 ms      2 ms      1 ms      223.4.0.146
  5   0 ms      1 ms      2 ms      223.4.0.195

Trace complete.

C:\>
```
--------------------------------------------------------
PC1 (RSales) to PC63 (SnM) via:  
RSalesSwitch - RSalesRouter - MainRouter -
MainF1Switch - MainF2Switch
```
C:\>ping 223.4.0.66

Pinging 223.4.0.66 with 32 bytes of data:

Reply from 223.4.0.66: bytes=32 time=5ms TTL=126
Reply from 223.4.0.66: bytes=32 time=1ms TTL=126
Reply from 223.4.0.66: bytes=32 time=1ms TTL=126
Reply from 223.4.0.66: bytes=32 time=5ms TTL=126

Ping statistics for 223.4.0.66:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 1ms, Maximum = 5ms, Average = 3ms

C:\>tracert 223.4.0.66

Tracing route to 223.4.0.66 over a maximum of 30 hops: 

  1   1 ms      0 ms      0 ms      223.4.0.113
  2   0 ms      1 ms      0 ms      223.4.0.138
  3   0 ms      0 ms      1 ms      223.4.0.66

Trace complete.

C:\>
```
--------------------------------------------------------
PC1 (RSales) to ISPRouter (ISP) via:  
RSalesSwitch - RSalesRouter - MainRouter -
CentralRouter - ISPouter
```
C:\>ping 200.200.100.2

Pinging 200.200.100.2 with 32 bytes of data:

Reply from 200.200.100.2: bytes=32 time=3ms TTL=252
Reply from 200.200.100.2: bytes=32 time=3ms TTL=252
Reply from 200.200.100.2: bytes=32 time=3ms TTL=252
Reply from 200.200.100.2: bytes=32 time=21ms TTL=252

Ping statistics for 200.200.100.2:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 3ms, Maximum = 21ms, Average = 7ms

C:\>tracert 200.200.100.2

Tracing route to 200.200.100.2 over a maximum of 30 hops: 

  1   0 ms      1 ms      0 ms      223.4.0.113
  2   1 ms      1 ms      0 ms      223.4.0.138
  3   0 ms      0 ms      1 ms      223.4.0.142
  4   1 ms      3 ms      2 ms      200.200.100.2

Trace complete.

C:\>
```
--------------------------------------------------------
PC11 (admin) to Server (Server) via:  
AdminSwitch - AdminRouter - Switch - CentralRouter - MainRouter - MainF1Switch
```
C:\>ping 223.4.0.98

Pinging 223.4.0.98 with 32 bytes of data:

Reply from 223.4.0.98: bytes=32 time=2ms TTL=125
Reply from 223.4.0.98: bytes=32 time=1ms TTL=125
Reply from 223.4.0.98: bytes=32 time=1ms TTL=125
Reply from 223.4.0.98: bytes=32 time=3ms TTL=125

Ping statistics for 223.4.0.98:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 1ms, Maximum = 3ms, Average = 1ms

C:\>tracert 223.4.0.98

Tracing route to 223.4.0.98 over a maximum of 30 hops: 

  1   0 ms      0 ms      0 ms      223.4.0.193
  2   0 ms      0 ms      0 ms      223.4.0.145
  3   0 ms      0 ms      2 ms      223.4.0.141
  4   0 ms      0 ms      1 ms      223.4.0.98

Trace complete.

C:\>
```