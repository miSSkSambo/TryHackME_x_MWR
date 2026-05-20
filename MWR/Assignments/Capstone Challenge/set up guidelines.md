# MWR CyberSec Capstone — Set up guide 

---

# STEP 1 — Start the TryHackMe Machines

Start the following machines:

- AttackBox
- Target Machine

Make sure:
- AttackBox status = Connected
- Target Machine status = ON

<img width="827" height="572" alt="image" src="https://github.com/user-attachments/assets/5b92b09b-099c-46af-a2e3-8f9269e19527" />


Locate the target IP address.


Example:

```bash
10.80.162.30
```

---

# STEP 2 — Add the Target to `/etc/hosts`

Open a terminal in Kali Linux.

Run:

```bash
echo "10.80.162.30 interns.mwrcybersec.loc" | sudo tee -a /etc/hosts
```

<img width="872" height="205" alt="image" src="https://github.com/user-attachments/assets/d203f8ec-bb04-4382-aeef-2418c677fb4d" />


Replace the IP with YOUR target IP.

<img width="966" height="376" alt="image" src="https://github.com/user-attachments/assets/2bc4577a-cae8-44f5-94e9-1bac39d5e0f1" />

Verify:

```bash
cat /etc/hosts | grep interns
```

Expected output:

```bash
10.80.162.30 interns.mwrcybersec.loc
```


---

# STEP 3 — Verify Connectivity

Run:

```bash
ping interns.mwrcybersec.loc
```
<img width="851" height="138" alt="image" src="https://github.com/user-attachments/assets/6e232ca6-44c7-4792-b9a9-525b2b00a2a0" />

If you receive replies:
✅ The target resolves correctly.

---

# STEP 4 — Open the Internship Portal

Open Firefox.

Go to:

```text
http://interns.mwrcybersec.loc
```

You should see the MWR CyberSec Internship Application Portal.

<img width="718" height="542" alt="image" src="https://github.com/user-attachments/assets/3f400490-468b-49b2-ad0c-aeb36df881c4" />

---

# STEP 5 — Verify TryHackMe Username

Open:

```text
https://vintern.thinkgreencorp.net
```
<img width="635" height="517" alt="image" src="https://github.com/user-attachments/assets/741f24b1-e6bc-4f16-8352-486164fbd837" />


Verify your TryHackMe username is registered.

<img width="665" height="510" alt="image" src="https://github.com/user-attachments/assets/85597b39-9678-4c0d-9ad8-9b3b8fccdad7" />

---

# STEP 6 — Activate the Exam Configuration

Open:

```text
http://interns.mwrcybersec.loc/exam/setup?token=35d66a3d01016ae21f99806a80bab5a4
```

<img width="743" height="492" alt="image" src="https://github.com/user-attachments/assets/45236737-3766-4b69-987a-2e8404174eee" />

Enter your TryHackMe username.

Click:

```text
Generate Config
```

<img width="592" height="270" alt="image" src="https://github.com/user-attachments/assets/4d264847-8e34-40bd-aa43-9c25c2006cf7" />

Wait for the success confirmation.

---

# STEP 7 — Start Burp Suite

Open a terminal.

Run:

```bash
burpsuite
```

When Burp opens:

- Temporary Project
- Use Burp Defaults
- Start Burp

---

# STEP 8 — Configure Firefox Proxy

In Firefox:

```text
Settings → Network Settings
```
<img width="638" height="478" alt="image" src="https://github.com/user-attachments/assets/76960e44-b1cc-4e02-a05d-edeb639a5449" />

Search:

```text
proxy
```
<img width="830" height="448" alt="image" src="https://github.com/user-attachments/assets/8271b6ad-eb16-4ef4-bc5c-7d7c47f85592" />

Select:

```text
Manual proxy configuration
```

Configure:

| Setting | Value |
|---|---|
| HTTP Proxy | 127.0.0.1 |
| Port | 8080 |

Tick:

```text
Also use this proxy for HTTPS
```
<img width="987" height="640" alt="Screenshot 2026-05-20 120055" src="https://github.com/user-attachments/assets/649be4f4-410d-47ea-bb04-99352a10bd79" />


Click:

```text
OK
```

Should it not work swtich to no proxy
<img width="442" height="135" alt="image" src="https://github.com/user-attachments/assets/6d5931bd-94e0-42c5-a46b-152d596f0327" />

---

# STEP 9 — Disable Burp Interception

In Burp:

```text
Proxy → Intercept
```

Ensure:

```text
Intercept is off
```

This prevents Firefox from freezing.

---

# STEP 10 — Test the Proxy

In Firefox visit:

```text
http://example.com
```

In Burp open:

```text
Proxy → HTTP History
```

If requests appear:
✅ Burp is working correctly.

---


# STEP 11 — Open Developer Tools

Press:

```text
F12
```

Open:

```text
Network
```

Tick:

```text
Preserve Log
```

---

# STEP 13 — Register an Account

Click:

```text
Register
```

Create a test account.

Example:

```text
Email: ********.com
Password: Pas************
```
<img width="730" height="593" alt="image" src="https://github.com/user-attachments/assets/17b7d47c-2789-4338-a1bc-55d7923ba354" />

Watch the registration request carefully.

Look for:
- role fields
- admin fields
- hidden parameters

---

# STEP 14 — Login

Login using the account you created.

Observe:
- Request body
- Response
- Tokens
- Cookies
- API endpoints

Common endpoints:

```text
/api/v1/auth/login
/api/v1/auth/register
```

<img width="633" height="583" alt="image" src="https://github.com/user-attachments/assets/a8371e49-6575-4557-81f4-b2e0bf2786a7" />

---



