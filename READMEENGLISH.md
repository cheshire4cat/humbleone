# HUMBLE ONE – Discord Fleet Controller (DEMO)

Humble One is an advanced Discord account fleet management center (self-bots), designed for high performance, stability, and a clean user interface (hUmble UI).  
The DEMO version showcases key connection management and fleet control mechanisms.

---

## Key Features of the DEMO Version

### 1. Sequential Strike Force (Join System)
Humble One uses a sequential joining algorithm instead of standard parallel methods. Accounts join one by one with precise delays (Stagger Join), increasing connection stability without requiring proxies.

- **Invite Handling:** automatically detects channel link or ID  
- **Auto-Guild Join:** automatically joins the server before entering a voice channel  

### 2. Unkickable Protocol (Auto-Rejoin)
Monitors session status in real-time. If an account is kicked from a channel, it reconnects immediately.  
Disconnects occur only when commanded by the user.

### 3. Fleet Manager and Account Control
Integrated panel for controlling all accounts at once:

- **Mute/Deafen All** – syncs microphones and headphones  
- **Instant Disconnect** – immediately disconnects all sessions  
- **Real-time Status** – live account activity monitoring  

### 4. Real-time Telemetry
Statistics panel updates every second, showing:

- resource usage  
- API latency  
- application uptime  

---

## Security and Technology

- **Code Obfuscation:** protects the code (CFF, RC4, SE)  
- **Portable EXE:** runs without installation, includes all necessary libraries  
- **Local Storage Persistence:** can remember tokens and login data  

---

## Running the DEMO Version

1. Download `Humble One 0.0.2.exe` from the release  
2. Launch the application  
3. Log in using the demo key available on Discord: [https://discord.gg/WsCPzHZ79P](https://discord.gg/WsCPzHZ79P)  
4. In Settings, enter tokens (limit: 5 in the demo)  
5. In Fleet, provide the invite link or channel ID and click “Deploy” (initial token initialization may be required)  

![Demo Screenshot](https://github.com/user-attachments/assets/e619c4ab-11ac-4eba-bf68-271c89eb11dd)

---

## Full Version (Coming Soon)

The DEMO is a limited version of the system. The full version will include:

- extended operational mechanisms (e.g., each account on a different proxy)  
- advanced audio management  
- no account limit  
- cloud configuration synchronization  
- additional fleet optimization and management features (including flood/massdm)  

---

## System Requirements and Dependencies – Humble One

### Operating System
- Windows 10 or newer (64-bit)  
- Alternatively macOS / Linux for the developer version (Node.js)

### Hardware
- CPU: minimum 4 cores  
- RAM: 8 GB or more (16 GB recommended for larger fleets)  
- Disk: at least 500 MB free space  
- Stable internet connection

### Software and Dependencies
- **Node.js:** version 18 or higher  
- **npm:** package management for Node.js (usually included with Node.js)  
- **FFmpeg:** for audio handling (built-in in portable EXE)  
- **Sodium (libsodium):** for audio and token encryption (built-in in EXE)  

### Permissions
- Ability to run `.exe` files  
- Internet access (TCP/UDP ports for Discord API)  
- Access to local file system to store tokens (if "Remember Credentials" is enabled)  

### Optional (Developer Environment)
- Git – to clone the repository from GitHub  
- Code editor, e.g., Visual Studio Code  
- Terminal / PowerShell / CMD for running Node.js scripts  

### Notes
- DEMO version supports up to 5 tokens.  
- Full version supports hundreds of tokens with proper Settings configuration.  
- The creator is not responsible for use outside educational and testing purposes.

### VirusTotal

![VirusTotal Screenshot](https://github.com/user-attachments/assets/e1ba1155-5b82-44a5-a00a-5667f1b6a2cb)

- [VirusTotal Check](https://www.virustotal.com/gui/file/c6703929fac78649890d1ea465e8e4cecf6b15afce3c7f7ff8e954dfcb3907d8?nocache=1)

---

© 2026 Humble One. All rights reserved.

Humble One is released under the MIT License. Use is allowed for educational, testing, and lawful purposes only. The creator is not liable for any damages resulting from misuse.
