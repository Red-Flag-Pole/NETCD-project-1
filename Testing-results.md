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