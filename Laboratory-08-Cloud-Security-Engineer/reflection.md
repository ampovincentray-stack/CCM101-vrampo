# Mission 8 Reflection: The Cloud Security Engineer

Through this laboratory activity, I learned that securing a cloud server requires more than simply deploying an application. A host-based firewall provides another layer of protection because it controls network traffic directly on the server. Even if an attacker gets past the physical network perimeter, the firewall can still block unauthorized incoming connections according to its rules.

Managing open network ports is important because every exposed service can become a possible entry point for attackers. By allowing only the ports required by the application, administrators can reduce the server's attack surface. In this activity, I allowed SSH for administration and TCP port 8080 for the web application while applying a default-deny incoming policy. This helped me understand the importance of allowing only necessary connections.

In a real enterprise environment, leaving MySQL port 3306 open to the public internet is dangerous because attackers may attempt password guessing, exploit database vulnerabilities, or try to access sensitive information. Database access should normally be restricted to trusted application servers or authorized networks. Strong authentication and additional security controls are also necessary.

This mission changed my perspective because I realized how easily an application can become exposed when its network security is not configured properly. Running the Nginx container was only one part of the task; checking the firewall status and creating specific rules were equally important. I also learned that testing an application locally does not always prove that external traffic is being filtered correctly.

Finally, having eight completed missions in my GitHub Cloud Computing Portfolio helps me organize my learning progress and demonstrate the skills I have practiced. Documenting my commands, saving screenshots, and explaining my results make my work easier to review. This activity taught me that cloud security is a continuous responsibility that requires careful configuration, verification, and regular monitoring.
