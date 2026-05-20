# MWR CyberSec Capstone — Step-by-Step Walkthrough

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

<img width="987" height="667" alt="image" src="https://github.com/user-attachments/assets/4cc8f288-84e6-4ee0-a329-2a90606b68b3" />


Replace the IP with YOUR target IP.

Verify:

```bash
cat /etc/hosts | grep interns
```

Expected output:

```bash
10.**.**.**.*0 interns.mwrcybersec.loc
```

---

# STEP 3 — Verify Connectivity

Run:

```bash
ping interns.mwrcybersec.loc
```

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

---

# STEP 5 — Verify TryHackMe Username

Open:

```text
https://vintern.thinkgreencorp.net
```

Verify your TryHackMe username is registered.

---

# STEP 6 — Activate the Exam Configuration

Open:

```text
http://interns.mwrcybersec.loc/exam/setup?token=35d66a3d01016ae21f99806a80bab5a4
```

Enter your TryHackMe username.

Click:

```text
Generate Config
```

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

Search:

```text
proxy
```

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

Click:

```text
OK
```

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

# STEP 11 — Install the Burp Certificate

In Firefox browse to:

```text
http://burp
```

Download:

```text
CA Certificate
```

Import it:

```text
Settings → Privacy & Security → Certificates → View Certificates → Authorities → Import
```

Tick:
- Trust this CA to identify websites

---

# STEP 12 — Open Developer Tools

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

---

# STEP 15 — Inspect Browser Storage

Open:

```text
Storage → Local Storage
```

and:

```text
Storage → Session Storage
```

Look for:
- JWT tokens
- accessToken
- refreshToken
- session values

---

# STEP 16 — Inspect Burp HTTP History

In Burp:

```text
Proxy → HTTP History
```

Watch for:
- `/api/`
- `/users`
- `/admin`
- `/applications`
- `/profile`

---

# STEP 17 — Send Interesting Requests to Repeater

Right-click requests.

Select:

```text
Send to Repeater
```

This allows:
- modifying requests
- replaying requests
- changing IDs
- testing authorization

---

# STEP 18 — Test IDOR Vulnerabilities

Example:

```text
/api/v1/users/1
```

Change:

```text
1 → 2
```

Look for:
- other users’ data
- unauthorized access
- hidden information

---

# STEP 19 — Test Admin Access

Try manually browsing to:

```text
/admin
/api/v1/admin
/dashboard/admin
```

Check for:
- admin dashboards
- unauthorized access
- sensitive information

---

# STEP 20 — Test Hidden Endpoints

Try:

```text
/swagger
/api-docs
/openapi.json
/debug
/internal
```

---

# STEP 21 — Test JWT Tokens

If a JWT token exists:

Inspect:
- role
- userId
- permissions
- admin values

Look for weak validation.

---

# STEP 22 — Test Role Manipulation

If requests contain:

```json
"role":"user"
```

Try:

```json
"role":"admin"
```

---

