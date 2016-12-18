---
layout: docs
title: 1d. Joining the server
permalink: /docs/1/d-joinserv/
---
You can connect to our server by typing or pasting the domain "shadow.ga" into their Direct Connect box. Some servers require the port `25565` or something
similar for the connection to work.

If your custom client or script requires entry of the port, using `25565` will result in a dead connection error. You must use the port `25579` if needed.
The server accomplishes this by using SRV records, which rid of the requirement to use ports for connecting to the game in order for a more user-friendly experience.
