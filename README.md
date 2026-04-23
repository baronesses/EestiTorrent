# 🏴‍☠️ Eesti Torrent (P2P Downloader)

![Version](https://img.shields.io/badge/Version-v4.0-blueviolet)
![Status](https://img.shields.io/badge/Status-Stable-brightgreen)
![Category](https://img.shields.io/badge/Category-Networking_%26_P2P-blue)

## 📌 Overview
**Eesti Torrent** is a custom-built, lightweight Peer-to-Peer (P2P) file transfer application optimized for secure private networks and Virtual LANs (such as Radmin VPN or Hamachi). It bypasses traditional cloud storage limits, allowing direct, high-speed file sharing between machines.

Featuring a sleek GUI, dynamic bandwidth control, and a robust multi-threaded download engine powered by `curl`, it ensures fast and uncorrupted data transfer via chunk hashing.

## ✨ Key Features

### 📡 Server Mode (Seeding)
* **One-Click Hosting:** Easily select any local directory and instantly host it on a specified port (default range: 8420-8500).
* **Multi-Instance Support:** Run up to 80 concurrent server instances.
* **Live Connection Journal:** Real-time logging of incoming connections, active ports, and client requests.
* **Process Management:** Built-in tools to monitor and safely kill specific seeding processes.

### 📥 Client Mode (Downloading)
* **Multi-Threaded Engine:** Utilizes `curl` under the hood for parallel chunk downloading, maximizing network bandwidth.
* **File Integrity:** Implements hash-checking to ensure downloaded files are perfectly assembled and uncorrupted.
* **Dynamic Speed Limiting:** Adjust the download speed (MB/s) in real-time without pausing or restarting the transfer (Set to `0` for uncapped speed).
* **Direct Fetching:** Target specific files using their exact extension names (e.g., `project_build.zip`).

## 🛠️ Tech Stack
* **Language:** Python
* **GUI Framework:** CustomTkinter
* **Network & Transfer:** HTTP/Sockets, `cURL` API, Multi-threading
* **Security:** Cryptographic Hashing for integrity checks
