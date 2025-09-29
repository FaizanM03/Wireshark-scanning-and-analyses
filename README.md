# Wireshark-scanning-and-analyses
Here’s a **short and clean version** you can add to your **GitHub profile README** or a project `README.md`:

---

### 🐧 Packet Capture & Analysis with Wireshark (Linux)

Capture and analyze network traffic on Linux using **Wireshark** and **tcpdump**.

#### ⚙️ Setup

```bash
sudo apt install wireshark -y
sudo usermod -aG wireshark $USER
```

> Log out and log back in after adding your user to the group.

#### 📡 Capture Options

* **Wireshark GUI**:
  Launch Wireshark → Select interface → Start capture

* **CLI with tcpdump**:

```bash
sudo tcpdump -i eth0 -w capture.pcap
```

Then open in Wireshark:

```bash
wireshark capture.pcap &
```

#### 🔍 Common Filters

```text
ip.addr == 192.168.1.1       # Filter by IP
tcp.port == 80               # HTTP traffic
dns                          # DNS traffic
http.request                 # HTTP requests
```

#### 💾 Save & Export

Use `.pcap` files to save, share, or analyze later.

---

