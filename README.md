sed
===

Requirement:


I want to remove the occurances of "Actual message:::" from file test.txt, except first occurrence 
(The first occurrence may be on any line, not necessary to be on line no 2). 
And also want that the message that is following "Actual message:::" is appended to the previous line. 
How can I achieve it using sed?? Can anyone please help me?

cat test.txt:
SUCCESSFULL1
Actual Message:::Searched Leased IP Not Found
No Leased IP Found
eth1 Link encap
Actual Message:::Ethernet HWaddr 00:90:FB:38:2D:41
inet addr
Actual Message:::172.16.5.43 Bcast:172.16.7.255 Mask:255.255.252.0


What I want is:
SUCCESSFULL1
Actual Message:::Searched Leased IP Not Found
No Leased IP Found
eth1 Link encap Ethernet HWaddr 00:90:FB:38:2D:41
inet addr 172.16.5.43 Bcast:172.16.7.255 Mask:255.255.252.0
