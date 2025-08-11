# Task 5: Capture and Analyze Network Traffic Using Wireshark

## Objective
Capture live network packets and identify basic protocols and traffic types using Wireshark.

## Tools Used
- **Wireshark** (Free and open-source network protocol analyzer)
- Operating System: Windows / Linux / macOS

## Deliverables
- `.pcap` file of captured traffic
- Short report of identified protocols and packet details
- README file with steps & screenshots

---

## Steps Performed

### Step 1 – Preparation & Permission Check
1. Closed heavy applications to avoid noisy traffic.
2. Ran Wireshark with administrator/root permissions.
3. Verified **Npcap** (Windows) or capture permissions (Linux/macOS) were installed.
4. Identified active network interface (e.g., `Wi-Fi`).
5. Created folder to save captures.
6. Ensured permission to capture on this network.

📸 **Screenshot:** `interface-selection.png` – showing selected network interface in Wireshark.

---

### Step 2 – Select the Network Interface
1. Opened Wireshark home screen.
2. Selected the active interface (Wi-Fi in our case).
3. Double-clicked to start capturing packets.

📸 **Screenshot:** `start-capture.png` – capturing live traffic.

---

### Step 3 – Apply a Capture Filter (TCP)
1. Stopped current capture.
2. Set **Capture Filter** to `tcp`.
3. Restarted capture.
4. Opened a website to generate TCP traffic.

📸 **Screenshots:**
- `tcp-capture-filter.png` – showing the capture filter set to `tcp`.
- `tcp-packets.png` – list of captured TCP packets.

---

### Step 4 – Apply a Display Filter (HTTP)
1. Kept capture running or started new capture.
2. Entered `http` in the **Display Filter** bar.
3. Visited a non-HTTPS website (`http://example.com`).

📸 **Screenshots:**
- `http-display-filter.png` – showing the HTTP display filter applied.
- `http-packets.png` – showing only HTTP packets.

---

### Step 5 – Follow a TCP Stream
1. Right-clicked any HTTP GET request.
2. Chose **Follow → TCP Stream**.
3. Viewed conversation between browser and server.

📸 **Screenshots:**
- `follow-tcp-stream-option.png` – right-click menu showing Follow → TCP Stream.
- `tcp-stream-window.png` – TCP Stream conversation view.

---

### Step 6 – Save TCP Stream Data
1. In TCP Stream window, set **Show data as** → ASCII.
2. Clicked **Save As** → `tcp-stream-data.txt`.
3. Closed the TCP Stream window.

📸 **Screenshot:** `save-tcp-stream-data.png` – save dialog with filename.

---

### Step 7 – Analyze HTTP Packet Details
1. Selected an HTTP GET request packet.
2. Expanded **Hypertext Transfer Protocol** in the middle panel.
3. Recorded **Request Method**, **Request URI**, **Host**.

📸 **Screenshot:** `http-get-request-details.png`

---

