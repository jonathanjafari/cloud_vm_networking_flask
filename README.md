# Flask on Cloud VM (Assignment 2)

**Student Info**  
Name: Jonathan Jafari  
Cloud Provider: Google Cloud Platform (GCP)  
Video Recording: [Click here to watch](PASTE_YOUR_LOOM_OR_ZOOM_LINK_HERE)  

---

## Steps

### 1. VM Creation
Created a VM instance on GCP using Ubuntu LTS.  
- Smallest free-tier instance was used.  
- A static external IP was assigned.  

![Screenshot 1](screenshots/screenshot1.png)

---

### 2. Networking (Port 5003 Open)
Configured a VPC firewall rule to allow inbound TCP traffic on port 5003, ensuring external access to the Flask app.  

![Screenshot 2](screenshots/screenshot2.png)

---

### 3. OS Update + Python Install
Updated and upgraded the OS, then installed Git, Python, pip, and venv.  

```bash
sudo apt update && sudo apt upgrade -y
sudo apt install -y git python3 python3-pip python3-venv
```

---

### 4. Flask App Setup (Virtual Environment + Requirements)
Cloned the class Flask starter repo, created a virtual environment, activated it, and installed requirements.

```bash
git clone https://github.com/hantswilliams/HHA-504-2025-FlaskStarter.git
cd HHA-504-2025-FlaskStarter
python3 -m venv venv
source venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

---

### 5. Flask App Running in Terminal
Edited `app.py` to run on `0.0.0.0:5003`, then launched Flask.

```bash
python3 app.py
```

![Screenshot 5](screenshots/screenshot5.png)

---

### 6. Flask App Accessible via Public IP
Tested the app in a browser using the VM's external IP and confirmed it loaded successfully.

**URL:**
```
http://<YOUR_PUBLIC_IP>:5003
```

![Screenshot 6](screenshots/screenshot6.png)

---

### 7. (Bonus) Domain Name Setup
Registered a free `.me` domain through the GitHub Student Pack with Namecheap.  
Added an A record pointing to the VM's external IP.

**Domain:**
```
http://hha504flaskdemo.me:5003
```

#### 7a. DNS Settings
![Screenshot 7a](screenshots/screenshot7a.png)

#### 7b. Flask App via Custom Domain
![Screenshot 7b](screenshots/screenshot7b.png)

---

## ✅ Assignment Outcomes
- Successfully deployed a Flask application on a cloud VM (GCP).
- Configured networking/firewall rules to allow public access on port 5003.
- Installed and managed dependencies via Python virtual environment.
- Verified accessibility both via public IP and a custom domain (bonus).
