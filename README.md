# CSE-421_computer-networks-project
End of the Experiment
In a chaotic suburban neighborhood, Malcolm and his family realized that
their communication setup across home, school, workplace, and other important
locations was completely unorganized. Since smooth communication is essential
for coordinating their daily activities and avoiding total confusion, Malcolm
decided to design a structured and secure network infrastructure connecting all
major zones associated with the family.
The goal is to establish a reliable communication topology among all of
these locations so that data can be exchanged efficiently, services can be hosted
properly, and all parts of the network remain reachable.
The main zones are associated with the following characters and locations:
• Malcolm’s School Lab (Malcolm) (840 hosts)
• Francis’s Military Academy Network (Francis) (390 hosts)
• Hal’s Workplace Office (Hal) (72 hosts)
• Reese’s Kitchen Control Zone (Reese) (210 hosts)
• Dewey’s Creative Experiment Lab (Dewey) (300 hosts)
In addition, the family home network has a committee of 25 devices/users
that must remain connected with all other zones.
Requirements:
1. The base network address must be derived from your Student
ID. You must clearly show how the network address was formed and then
perform VLSM subnetting.
2. The family home network will contain a web server and a DNS server.
A dedicated server named WilkersonHub must display:
"Life is unfair... but the network works!"
3. The family home network must use static IP addressing.
4. All other networks must use DHCP, configured as follows:
• Router-based DHCP:
– Malcolm’s School Lab
– Reese’s Kitchen Control Zone
• Server-based DHCP:
– Francis’s Military Academy Network
– Hal’s Workplace Office
– Dewey’s Creative Experiment Lab
1
5. Malcolm’s School Lab and Dewey’s Creative Experiment Lab must each
have an email server, and email communication must be established
between them.
6. The following direct router-level connections must be established:
• (Francis’s Military Academy - Reese’s Kitchen Zone)
• (Hal’s Workplace - Malcolm’s School Lab)
These connections must use different routers.
7. All networks must be interconnected using the minimum reasonable
number of routers.
Routing and Connectivity Constraints:
1. Dynamic Routing: The networks of Malcolm’s School Lab, Reese’s
Kitchen Zone, and Hal’s Workplace must be connected using a dynamic routing protocol (e.g., RIP).
2. Static Routing Configuration:
The following static routing types must be configured explicitly between
the specified networks:
• Standard Static Routes: Must be configured between:
– Francis’s Military Academy Network ↔ Family Home Network
• Default Static Route: Must be configured on the Family Home
router to forward all unknown traffic toward:
– Malcolm’s School Lab Network
Summary static routes and fully specified static routes are not allowed.
3. Floating Static Route: A floating static route must be configured between the Family Home and Dewey’s Lab via Malcolm’s School Lab
with an AD of 25.
4. Hybrid Router Requirement: The router connecting Malcolm’s School
Lab must be configured with both dynamic routing and static routing.
5. At least two end devices per network must be shown.
6. Full connectivity must be verified using ping between any two networks.
2
Deliverables:
The entire network described above should be implemented in Cisco Packet
Tracer using appropriate devices such as routers, switches, servers, PCs, laptops, and any other required components, along with complete configuration of
addressing, routing, and services.
You must submit the following:
1. A network topology diagram (screenshot) with clear and proper labels
for all routers, switches, servers, and end devices.
2. The configuration commands of all the routers you have implemented (for example, as text output from Packet Tracer’s CLI or copied
from the running configuration).
3. A complete VLSM tree showing how you subnetted the chosen network
address to satisfy all host requirements with minimal address waste.
4. An IP address table summarizing:
• Subnet addresses and masks
• Default gateways for each network zone
• Assigned IP addresses of servers and example end devices
• Router interface IPs and their corresponding networks
5. A short explanation showing how the base network address was derived from your Student ID.
6. A brief note identifying:
• which network used router based DHCP
• which network used server based DHCP
• which routers used static routing
• which part of the network used dynamic routing
• which router used both static and dynamic routing

