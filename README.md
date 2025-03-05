# Multi-Session Plex Killer

<h2 align="center">Want to Help? Click the Star in the Upper-Right Corner! ⭐</h2>

**Purpose**  
If you run multiple Plex servers and want to limit how many concurrent streams a particular user can have *across all servers*, this script can help. Simply set a threshold (e.g., 2 total streams), and if a user exceeds it (e.g., 3 streams across any combination of servers), the script will terminate all of their active sessions.

## How It Works

- **Multi-Server Aware:** The script connects to multiple Plex servers (via Tautulli) to check each user’s total streams.  
- **User Threshold:** You decide how many total streams a user is allowed (e.g., 2). If they exceed it, the script automatically kills their sessions.  
- **Easy Deployment (Unraid):** If you’re on Unraid, simply place the script in the **User Scripts** plugin and schedule or run it as needed.  
- **Custom Message:** When a user is forced off, they’ll see a warning message indicating they exceeded the global limit.

## Versions

v1: Initial Script
v2: Added to Exempt User(s)

## Quick Start

1. **Download the Bash script:**  
   [plex-session-killer.sh](plex-session-killer.sh)

2. **Set Threshold & Server Info:**  
   - Edit the script to specify:
     - Your Tautulli or Plex server details (API keys and URLs)
     - The maximum allowed streams per user.

3. **Run on Unraid (Optional):**  
   - Go to **User Scripts** (on Unraid)  
   - Upload or paste the script  
   - Set to schedule on startup

## Log Output

The script logs each check and displays:
- How many sessions each user has  
- Whether they exceeded the threshold  
- Any termination actions taken

![Log Explanation](https://github.com/user-attachments/assets/a26df424-c921-44b9-adbe-a8957a549353)

## Example Termination Message

When a user is forced to stop their streams, they’ll see a prompt similar to this:

![Termination Prompt](https://github.com/user-attachments/assets/78231819-381f-4291-8122-9537abf9ee5b)

---

**Stay tuned** for more features and updates! 
