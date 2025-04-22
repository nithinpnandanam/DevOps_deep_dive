>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
I have 5 teams who are working on 5 different applications
So I bought 5 servers .
Each server is given to each team.
Each server has a spec of 100GB RAM and 100 core
Team 1 uses server 1
Team 1 has deployed its application on server 1
This application only need 4GB RAM and 4 processors
Hence there is inefficiency
Most of the specs of the server 1 is unutilised 
Thus inefficiency comes into picture
This is the similar case for all the other servers
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
Solution
Refer Image 1
We have a physical server that we bought from IBM
In that physical server we install Hypervisor
Hypervisor is a software for installing virtual machines on a physical server
Memory CPU Hardware are unique for each Virtual machine by logical isolation
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
Refer Image 2
A data center has many physical servers
Lets say each physical server has 100 GB of Ram and 100 Core
Using aws CLI or AWS UI I am requestiong for a vm haning 10 GB Ram and 12 core
AWS receive the request and looks for Physical servers that is ideal for the requirement
If P1 is already occupied and say P100 is free then that physical server will be considered.
But P100 has 1000GB RAM and 1000 core
AWS send request to the Hypervisor and and we get a VM in return.
Actually we get all the details to access a virtual machine like IP address 

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>