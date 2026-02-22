# UnRAID UniFi Toolkit Installation Guide

Follow these steps to get the UniFi Toolkit up and running on your UnRAID server.

---

### 1. Install UI Toolkit
Open your UnRAID dashboard, navigate to the **Apps** tab, search for **UI Toolkit**, and install it.

### 2. Configure Permissions & Encryption
Open your **Terminal** and execute the following commands to set the correct folder permissions and generate a unique encryption key:

```bash
# Set folder permissions
chown 1000:1000 /mnt/user/appdata/unifi-toolkit

# Generate your unique Encryption Key
docker run --rm python:3-slim sh -c "pip install -q cryptography && python -c 'from cryptography.fernet import Fernet; print(Fernet.generate_key().decode())'"
```

[!IMPORTANT]
 Copy the last line of the output from the terminal. Go back to your Docker template, paste it into the field labeled "Encryption Key", and click Apply.

### 3. Finalize Setup

To complete the configuration, follow the detailed walkthrough provided by Crosstalk Solutions in the video below:

* Watch: [UniFi UI Toolkit Setup Guide](https://www.youtube.com/watch?v=7au0H_-PR4U)

---
Thanks to [filthy](https://forums.unraid.net/profile/127111-filthy/) on Unraid forum