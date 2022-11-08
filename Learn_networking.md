# -- **NETWORKING BASICS** --
- https://medium.com/@computerscienceengineering/basics-of-computer-networking-6c7b961f4e14
- https://www.youtube.com/watch?v=ZKhorleA5aA 
`All Concept clearing about ipconfig command Very Important`
<hr>

# Host and Nodes
1. <p style="color:Pink;">Host are basically client or server sending or receiving data to each other</p>
1. <p style="color:Pink;">Nodes are basically the intermediary devices that makes the connection between client and server.</p>

<p style="color:orange;">A node is also a broader term that includes anything connected to a network, while a host requires an IP address. In other words, all hosts are nodes, but network nodes are not hosts unless they require an IP address to function.</p>

<hr>

## What is a Hostname
 *A hostname is a plaintext name identifying a host in a given domain. On a local area network (LAN), a server's hostname might be a nickname like `mailserver1`. On the internet, a hostname makes up part of a web address and has three parts: `the subdomain`, `domain name` and `top-level domain`. For example, the hostname `whatis.techtarget.com` consists of the subdomain whatis, the domain techtarget and the top-level domain .com.*

 <hr>

 ## All About IP Addressing  (ip address, subnet mask, default gateway)
 - *Subnet Mask : -* 
    <p style="color:Pink;">Tells which part of network address refers to Network and host (255.255.255.0) (here 0 is the host also here 254 values are possible in a public ip)</p>
    <p style="color:lightblue;">In ip address each part seperated by (.) is an octet like which each has 255 possible value (0-255)</p> 

    Also in our `192.168.1.0` (private IP) the `0` is assigned for router's address and `255` is set for broadcaster it will broadcast the message to every connected device by the router.
    
    `192.168.1.0`
    
    [Public and Private IP **CLICK ME!**](https://www.tutorialspoint.com/difference-between-private-and-public-ip-addresses)
    
    <img src='https://i0.wp.com/ipwithease.com/wp-content/uploads/2018/07/img_5b5f52b5ec2f1.png?resize=708%2C401&ssl=1'>
    


-  *Default  Gateway : -* 
    <p style="color:yellow;">When the computer doesn't know the destination address that means the destination isn't available in the local networks so to send data to destination.. default gateway is sent a request and then it resolve everything for our computer</p>

 
- *IP Address : -* 
    <p style="color:rgb(234,23,128);">IP Address is basically a address which is assigned by the router to all its connected device (also known as logical address of the device)</p>

- *Mac Address : -*
    <p style="color:lightgreen;">Mac address is basically a address which is the physical address of a device that means the device owns it and it is given to it at the time of manufactoring</p>

- *Private IP nowadays : -*
    <p style="color:white;">Modems assigns the public ip or the internet's exact public ip to our system's but nowadays modems are connected to router or either router works only in our home so they assigns a private ip to our devices. </p>

- *Dynamic Host Configuration Protocol (DHCP)*
    <p style="color:aqua;">DHCP is a protocol that resolves or assigns ip address to our system devices connected to the router automatically.... actually router has this dhcp protocol feature in itself to assign ip's to connected devices</p> 

- *Domain Name System : -*
    <p style="color:magenta;">DNS, or the Domain Name System, translates human readable domain names (for example, www.amazon.com) to machine readable IP addresses (for example, 192.0.2.44).</p>

    Then there comes the topic of 
    `dns flush` (cached dns basically) basically to avoid 
    
    `dns spoofing` (changing cache dns for redirecting to malfunctioning websites by hackers) and 
    
    `diagonasing network`
    
     https://www.youtube.com/watch?v=ZKhorleA5aA 

 <hr>

## Some ipconfig commands for Windows
- `ipconfig /all`
- `ipconfig `
- `ipconfig /flushdns`
- `ipconfig /displaydns`
- `ipconfig /?`
 
<hr>

## what is a PORT
> <p style="color:hotpink;">Port can be referred to as a logical channel through which data can be sent/received to an application. Any host may have multiple applications running, and each of these applications is identified using the port number on which they are running.'</p>

> <p style="color:darkseagreen;">Ports are used to get the exact service asked by the client like web page, ftp from the server or system (request can be for server or for the system itself</p>

## Some Facts (should know) about Port
```
0- 65535		-- total available PORT's

0-1023		    -- Well known used port
1024-49151	    -- Can be company owned only
```
- above two are used to get services of server or like external from client

- 49152-65535	Private or dynamic used on client computer only

## Some common used PORT's and their usage in reality
```
443 stands for https website services
80 stands for http website services
21 stands for file transfer protocol services
```

## Netstat command inside Look 
-- (use netstat command with -n ) for more details

- local address section containing port more than 49152(private) shows the service being used like web page or browser service maybe which is temporarily assigned for usage
- although in foreign address section you will see :443 which is for https connection and 21 for ftp

## What is DNS
- dns is basically a server which resolves or converts our normal language address to the ip address for locating server for requesting data

## What is ARP (address resolution Protocol)
- arp is used to convert ip address to its corresponding physical address(MAC)


 