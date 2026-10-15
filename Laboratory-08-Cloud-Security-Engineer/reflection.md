# Mission Reflection: Securing a Cloud Server

This laboratory gave me practical experience in securing a Linux server with the Uncomplicated Firewall, also known as UFW. I learned that deploying a web application is only one part of managing cloud infrastructure. Administrators must also decide which network connections are necessary and prevent unwanted traffic from reaching the server.

A host-based firewall adds protection directly to a machine by controlling network traffic according to configured rules. If an attacker passes through an external network security layer, the server's firewall can still reject unauthorized connections. This additional protection supports the principle of defense in depth. It does not replace other security measures, but it provides an important barrier against unwanted access.

The number of open ports also affects server security. Every unnecessary service can create another opportunity for attackers to discover weaknesses. By allowing only the ports needed for administration and application access, administrators can reduce the attack surface and make the server easier to manage. Verifying the firewall rules helps ensure that the system follows the intended security policy.

Opening MySQL port 3306 to the public internet is especially risky because databases often contain sensitive information. Attackers could attempt unauthorized logins, exploit software vulnerabilities, or search for poorly secured database services. A safer design keeps the database on a private network and permits access only from authorized application servers.

One important lesson was to allow SSH before enabling the firewall. If SSH is blocked, remote administrators may lose access to the server. I also learned that commands such as `sudo ufw status verbose` and `sudo ufw status numbered` help verify the active configuration. Testing the web application provides additional evidence that the required service remains accessible.

My GitHub portfolio now shows my development across cloud infrastructure, containers, operations, and security. I understand better that a working server is not automatically a secure server. Cloud security requires planning, correct configuration, testing, and regular maintenance to reduce risks and protect important data.
