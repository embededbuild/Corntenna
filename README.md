<div align="center">

# 🌽 CORNTENNA

```text                                                                                 
                       [ LOCAL NETWORK RECON TERMINAL ]
```

*"The network talks. We just listen."*

Built on an ESP32 because laptops are expensive and curiosity is free.

</div>

---

## What is CORNTENNA?

CORNTENNA is a handheld network reconnaissance tool designed to map the digital neighborhood around you.

Plug it in.

Connect to a network.

Watch the devices reveal themselves.

Routers.
Phones.
Printers.
Smart TVs.
Mystery boxes with suspiciously open ports.

Every device leaves a trail.

CORNTENNA follows it.

---

## Features

### 📡 Wireless Recon

- Scan nearby Wi-Fi networks
- View signal strength
- Identify security types
- Interactive network selection

### 👁 Device Discovery

- ARP-assisted device detection
- Local subnet enumeration
- MAC address collection
- Live device inventory

### 🔍 Port Recon

Scans common services including:

```text
21   FTP
22   SSH
23   Telnet
80   HTTP
443  HTTPS
445  SMB
554  RTSP
8080 HTTP-Alt
8443 HTTPS-Alt
9100 Printer
```

### 🧬 Device Fingerprinting

Recognizes hardware vendors including:

- Apple
- Samsung
- Cisco
- Google
- Amazon
- Ubiquiti
- Netgear
- TP-Link
- Raspberry Pi
- Espressif
- Sony
- Microsoft
- Synology

### ⚡ Connection Intelligence

- RSSI monitoring
- Signal quality grading
- Gateway information
- Local IP information
- Subnet details

---

## Terminal Commands

```text
WIFI         Scan and connect
STATUS       Display connection info
SCAN         Discover devices
LIST         Show device inventory
DISCONNECT   Drop Wi-Fi connection
CLEAR        Clear discovered devices
PING         Test console response
```

---

## Example Session

```text
>> WIFI

[1] CoffeeShop_WiFi
[2] Home_Network
[3] Definitely_Not_FBI_Van

>> 2

>> Connected!

IP Address : 192.0.2.101

>> SCAN

>> Running TCP discovery...

>> Device: 192.0.2.10
>> Open ports: 80,443

>> Device: 198.51.100.22
>> Open ports: 22,80

>> Device: 203.0.113.7
>> Open ports: 9100

>> TCP discovery done

>> LIST

  +===================+==================+=============================+===========+==========+
  || MAC              || IP              || OPEN PORTS                || Device    || Source  |
  +===================+==================+=============================+===========+==========+
  || B8:3E:59:XX:XX:X || 192.0.2.10      || 80,443                    || Apple     || TCP     |
  || DC:A6:32:XX:XX:X || 198.51.100.22   || 22,80                     || Raspberry || TCP     |
  || A0:B3:CC:XX:XX:X || 203.0.113.7     || 9100                      || Printer   || TCP     |
  +===================+==================+=============================+===========+==========+
   Total: 3
```

---

## Hardware

```text
ESP32 Development Board
USB Cable
Serial Terminal
Questionable Sleep Schedule
```

---

## Build

### Requirements

- Arduino IDE
- ESP32 Board Package

### Libraries

```cpp
WiFi.h
esp_wifi.h
WiFiUdp.h
lwip/etharp.h
lwip/netif.h
lwip/tcpip.h
```

### Upload

```bash
git clone https://github.com/YOUR_USERNAME/CORNTENNA.git
```

Open in Arduino IDE.

```text
Board: ESP32 Dev Module
Baud: 115200
```

Compile.

Upload.

Observe.

---

---

## Philosophy

Networks are ecosystems.

Every device broadcasts a story.

Most people never notice.

CORNTENNA exists for the people who do.

Not because we want to break things.

Because we want to understand them.

---

## Legal

Only scan networks you own or have permission to analyze.

Don't be the reason your ISP sends weird emails.

---

<div align="center">

### WE ARE ALL JUST DEVICES ON SOMEBODY ELSE'S NETWORK.

🌽

</div>
