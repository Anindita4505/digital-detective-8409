# Mission 7 — How Computers Communicate

## 1. Mission Title

How Computers Communicate — Networking Fundamentals

## 2. Task / Objective

The objective of this mission was to understand basic networking concepts, observe network connectivity and DNS lookup information using Terminal, and explain what happens when a website is opened in a browser.

## 3. Work Completed

### Task 7.1 — Network Concepts

| Concept          | Explanation                                                                         | Example                        |
| ---------------- | ----------------------------------------------------------------------------------- | ------------------------------ |
| LAN              | A network covering a small geographical area, such as a home, laboratory or office. | Home Wi-Fi network             |
| MAN              | A network covering a city or a large campus area.                                   | City-wide university network   |
| WAN              | A network covering large geographical areas.                                        | Internet                       |
| DNS              | Translates domain names into IP addresses.                                          | Resolving example.com          |
| Router           | Connects networks and forwards data between them.                                   | Home Wi-Fi router              |
| Protocol         | A set of rules devices follow to communicate.                                       | HTTP, HTTPS and TCP            |
| Packet Switching | Data is divided into smaller packets that travel across a network.                  | Sending data over the internet |
| Client-Server    | A client requests a service and a server provides it.                               | A browser requesting a webpage |

### Task 7.2 — Network Information Observation

**Connectivity Test**

Command used:

`ping -c 4 example.com`

Observations:

- 4 packets transmitted.
- 4 packets received.
- 0% packet loss.
- Average response time: 21.983 ms.

A connectivity test checks whether a computer can reach another device or server over a network. The successful replies indicated that example.com was reachable during the test.

**DNS Lookup**

Command used:

`nslookup example.com`

Observations:

- DNS server: 8.8.8.8 (Google Public DNS).
- Domain queried: example.com.
- Returned IP addresses: 104.20.23.154 and 172.66.147.243.

A DNS lookup displays information about the IP address associated with a domain name. A domain may resolve to multiple IP addresses.

The DNS server helps translate a human-readable website name into an IP address so that a computer can communicate with the appropriate server.

### Task 7.3 — What Happens When You Open a Website?

1. The user enters a website address in a web browser.
2. DNS helps find the IP address associated with the domain name.
3. The computer establishes a network connection with the website's server through the network.
4. The browser acts as a client and sends an HTTP or HTTPS request using communication protocols.
5. The server receives and processes the request.
6. The server sends the requested webpage data back to the client.
7. The browser processes the response and displays the webpage to the user.

HTTPS also encrypts communication between the browser and server to help protect data.

## 4. Commands / Tools Used

| Command / Tool          | Purpose                                                              |
| ----------------------- | -------------------------------------------------------------------- |
| `ping -c 4 example.com` | Tests connectivity by sending four packets and checking for replies. |
| `nslookup example.com`  | Performs a DNS lookup to find IP addresses associated with a domain. |
| `git status`            | Checks the current Git repository status.                            |

Tools used: macOS Terminal and DNS lookup utility.

## 5. My Understanding

I learned that computer networks allow devices to communicate and share resources. LAN, MAN and WAN differ mainly in the geographical area they cover.

I understood that DNS translates domain names into IP addresses, routers forward network traffic, and protocols establish communication rules.

I also learned how packet switching divides data into smaller packets and how clients and servers communicate through requests and responses.

The connectivity test helped me understand how to check whether a website is reachable, while the DNS lookup showed how domain names are resolved into IP addresses.

## 6. Difficulties Faced

No major difficulties were faced while performing the network commands. Both the connectivity test and DNS lookup executed successfully.

## 7. How I Resolved Them

I followed the Terminal instructions and examined the outputs of both commands to understand the network connectivity and DNS resolution results.

## 8. Evidence / Files

- `mission-07-networking/README.md` — Contains the network concepts table, command observations, explanations and website communication steps.
- Terminal observations from `ping -c 4 example.com` and `nslookup example.com`.

No private IP address, Wi-Fi name or other identifying network details were included.

## 9. Commit Details

Planned commit message: `Explain networking concepts and website communication`

Branch: `main`

The mission documentation will be committed and pushed after reviewing the README.
