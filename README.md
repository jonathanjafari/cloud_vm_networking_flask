# Flask on Cloud VM (Assignment 2)

## Student Info
- **Name:** Jonathan Jafari  
- **Cloud Provider:** Google Cloud Platform (GCP)  
- **Video Recording (Zoom/Loom):** [Click here to watch](PASTE_YOUR_LINK_HERE)  

---

## Steps & Screenshots

### 1. VM Creation
Created a new VM instance in Google Cloud.  
![Screenshot 1](screenshots/screenshot1.png)

---

### 2. Firewall Rule Configuration
Configured a firewall rule to allow traffic on port **5003**.  
![Screenshot 2](screenshots/screenshot2.png)

---

### 3. OS Update + Python Install
Updated packages and installed Python, pip, and git.  
![Screenshot 3](screenshots/screenshot3.png)

---

### 4. Python Environment + Flask Install
Created a virtual environment, upgraded pip, and installed Flask dependencies.  
![Screenshot 4](screenshots/screenshot4.png)

---

### 5. Flask App Setup
Created `app.py` with a simple Flask app that returns an HTML page.  
![Screenshot 5](screenshots/screenshot5.png)

---

### 6. Flask App Running
Successfully started Flask on port **5003** and confirmed it was accessible.  
![Screenshot 6](screenshots/screenshot6.png)

---

### 7a. Domain Registration
Registered a free `.me` domain via Namecheap (through GitHub Student Pack).  
![Screenshot 7a](screenshots/screenshot7a.png)

---

### 7b. Domain DNS Setup
Configured DNS records to point the domain to the Google Cloud VM.  
![Screenshot 7b](screenshots/screenshot7b.png)

---

## Final Notes
- Flask app is accessible via the VM external IP on port **5003**.  
- Bonus: Linked a custom domain (Namecheap → GCP External IP).  

