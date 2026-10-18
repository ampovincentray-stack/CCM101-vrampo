# Mission 8 Reflection: The Cloud Security Engineer

Starting the cloud server is more difficult than starting the app itself, which made me conclude the same. A host firewall may block access to the server by blocking certain communications towards it, and this is especially true if somebody has already penetrated your network.

When open ports in a network are created, you are effectively creating entrances for intruders to gain access into your network. You must leave only necessary open ports on your server for the applications requiring them to function. In my lab, I opened TCP port 8080 for a web application and TCP port 22 for SSH administration. I also set up a default policy to deny all incoming connections.

For a business, doing this is really a bad and insecure idea. You should never expose your application's port 3306 to the internet. People will try to brute-force your MySQL database, hack it, or just steal data. You need to restrict your database access to only trusted application servers and specific network addresses.

This task altered my perspective as it came to me how prone an application can be if its network security is not correctly arranged. As pushing the Nginx container alone was not the solution, I also had to check if firewalls' status is correct and rules are created. What I learned is that testing an application in the network does not mean that application can filter out of network data correctly.

I’ve finished eight missions that can be found in my GitHub Cloud Computing Portfolio. This helps organize my knowledge and showcases the competencies I have gained. Taking notes about the commands, saving the screenshots, and explaining the results makes my work much simpler when I need to check what I’ve done.
