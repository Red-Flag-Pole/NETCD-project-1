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

Link between MainF1Switch and MainF2Switch is down
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

Do nslookup of "server" on dns server, Server (223.4.0.98)
-------------------------------------------------------
PC26 (RnD)