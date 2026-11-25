# Mission 7 — How Computers Communicate

## 1. Task / objective

The objective of this mission is to understand basic networking concepts, observe network connectivity and DNS information using Terminal, and explain how a website loads when a user enters its address in a browser.

## 2. Work completed

### Task 7.1 — Explain network concepts

| Concept                         | Explanation                                                                                                                                  | Example                                                                  |
| ------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------ |
| LAN (Local Area Network)        | A network that connects devices within a small geographical area.                                                                            | Computers connected in a home, office or college lab.                    |
| MAN (Metropolitan Area Network) | A network that connects devices or smaller networks across a city or large campus.                                                           | A network connecting different branches of an institution across a city. |
| WAN (Wide Area Network)         | A network that connects devices and networks across large geographical areas.                                                                | The Internet.                                                            |
| DNS (Domain Name System)        | A system that translates human-readable domain names into IP addresses.                                                                      | Finding the IP address associated with `example.com`.                    |
| Router                          | A networking device that connects networks and forwards data between them.                                                                   | A home Wi-Fi router connecting devices to the Internet.                  |
| Protocol                        | A set of rules that devices follow to exchange data.                                                                                         | HTTP, HTTPS and TCP.                                                     |
| Packet switching                | A method of communication in which data is divided into smaller packets that travel across a network and are reassembled at the destination. | Sending a file over the Internet.                                        |
| Client-server                   | A communication model in which a client requests a service and a server provides it.                                                         | A browser requesting a webpage from a web server.                        |

### Task 7.2 — Observe network information

**Connectivity test**

Command used: `ping -c 4 example.com`

Purpose: A connectivity test checks whether a device can reach another host over a network. It sends test packets and reports whether replies are received, along with information such as response time and packet loss.

**My observation:** The connectivity test to `example.com` was successful. All four packets were received, with 0% packet loss. The average round-trip response time was approximately 10.008 milliseconds. This confirms that my computer could reach the example domain during the test.

**DNS lookup**

Command used: `nslookup example.com`

Purpose: A DNS lookup displays information about how a domain name is resolved into IP addresses. It can show the DNS server used for the lookup and the address records returned for the domain.

**My observation:** The DNS lookup for `example.com` was successful. The DNS server used was `8.8.8.8`. The domain resolved to two IP addresses: `104.20.23.154` and `172.66.147.243`. The output showed a non-authoritative answer.

**Role of DNS:** DNS translates human-readable domain names into IP addresses, allowing browsers and other applications to locate servers.
When a user enters a website name in a browser, DNS helps find the IP address associated with that domain. The browser can then use that address to communicate with the website's server.

### Task 7.3 — What happens when you open a website?

1. The user enters a website address in a web browser. The browser acts as the client that requests information.
2. The browser checks whether it already knows the IP address for the domain. If necessary, it uses DNS to look up the address.
3. The device sends network traffic through its network connection and router towards the destination.
4. The client establishes communication with the website's server using appropriate network protocols, such as TCP and HTTPS.
5. The browser sends an HTTP request to the server asking for the webpage or another resource.
6. The server processes the request and sends a response containing the requested content or an error message.
7. The browser receives the response, processes the content and displays the webpage to the user.

## 3. Commands / tools used

| Command or tool         | Purpose                                                                             |
| ----------------------- | ----------------------------------------------------------------------------------- |
| `ping -c 4 example.com` | Sends four connectivity test packets to an example domain and displays the results. |
| `nslookup example.com`  | Looks up DNS information for the example domain.                                    |
| Terminal                | Used to execute networking commands and observe their output.                       |

## 4. My understanding

I learned that networks allow devices to communicate and share resources. LAN, MAN and WAN describe networks based on their geographical coverage. DNS helps translate domain names into IP addresses, while routers forward data between networks. Protocols define the rules of communication. Packet switching divides data into smaller packets, and the client-server model explains how a browser requests information from a server.

I also learned that opening a website involves several stages, including DNS lookup, network communication, a client request, a server response and browser rendering.

## 5. Difficulties faced

No major technical difficulties were faced while running the connectivity test and DNS lookup commands.

## 6. How I resolved them

I used the Terminal commands `ping` and `nslookup` to observe network connectivity and DNS resolution. I reviewed their outputs to understand the results.

## 7. Evidence / files

- `mission-07-networking/README.md` — Network concepts, command observations and website communication explanation.
- `evidence/mission-07-connectivity.png` — Connectivity test output.
- `evidence/mission-07-dns-lookup.png` — DNS lookup output.

## 8. Commit details

**Commit message:** `Explain networking concepts and website communication`
**Branch:** `main`
**Status:** 'Successfully committed and pushed to GitHub.'
