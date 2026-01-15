# LAB-03: Browser Fingerprinting (Kali Linux)

## 🎯 Objective
To understand how websites can identify and track users **without using IP addresses or cookies**, by analyzing browser, system, and behavioral characteristics.

This lab demonstrates **browser fingerprinting** using public testing tools.

---

## 🔹 Tool Used

- https://coveryourtracks.eff.org  
(Provided by the Electronic Frontier Foundation)

---

## 🔹 Step 1: Initial Fingerprinting Test

### Action
The test was performed using:
- OS: Kali Linux
- Browser: Firefox (default Kali browser)
- No VPN enabled

The option **“Test your browser”** was selected.

---

## 🔹 Example Test Results
# LAB-03: Browser Fingerprinting (Kali Linux)

## 🎯 Objective
To understand how websites can identify and track users **without using IP addresses or cookies**, by analyzing browser, system, and behavioral characteristics.

This lab demonstrates **browser fingerprinting** using public testing tools.

---

## 🔹 Tool Used

- https://coveryourtracks.eff.org  
(Provided by the Electronic Frontier Foundation)

---

## 🔹 Step 1: Initial Fingerprinting Test

### Action
The test was performed using:
- OS: Kali Linux
- Browser: Firefox (default Kali browser)
- No VPN enabled

The option **“Test your browser”** was selected.

---

## 🔹 Example Test Results

Your browser has a unique fingerprint


### Detected Information (Example)
Browser: Firefox 115 ESR
Operating System: Linux (Kali)
Platform: x86_64
Screen Resolution: 1920x1080
Timezone: Asia/Kolkata
Languages: en-US

### Fingerprinting Result


### Tracking Protection Result

Your browser blocks some tracking


---

## 🔹 Step 2: Behavioral & Interaction Signals

The test also analyzes **how the browser behaves**, including:

- JavaScript execution behavior
- Input event timing (keydown / keyup)
- Rendering differences
- Feature availability

### Important Clarification
- The website does **NOT** read what the user types
- It does **NOT** capture keystrokes or passwords
- Only **timing and behavior metadata** is observed

This technique is known as **behavioral fingerprinting**.

---

## 🔹 Why Kali Linux Stands Out

### Observation
The browser fingerprint is marked as **highly unique**.

### Explanation
- Kali Linux is rarely used for normal browsing
- Security-focused configurations reduce randomness
- Hardened browsers normalize values, making them stand out

### Defender Perspective
From a security standpoint:
- Rare environments are easier to classify
- Uncommon setups raise confidence in identification

---

## 🔹 Privacy Hardening Test (After Changes)

The following hardening steps were applied:
- Firefox Enhanced Tracking Protection: Strict
- `privacy.resistFingerprinting = true`
- uBlock Origin installed (default settings)

### Example Result After Hardening


Fingerprint: Still unique
Tracking Protection: Improved
Some values standardized



### Interpretation
- Hardening reduces tracking confidence
- Fingerprinting is **reduced but not eliminated**
- Uniqueness remains due to OS rarity

---

## 🧠 Key Concepts Learned

- Browser fingerprinting does not rely on IP addresses
- Cookies are not required for identification
- Behavioral signals increase tracking accuracy
- Privacy tools reduce risk but do not provide anonymity
- Kali Linux is a testing OS, not an anonymity platform

---

## ✅ Conclusion
This lab demonstrates that modern tracking relies on browser and behavioral characteristics rather than traditional identifiers like cookies or IP addresses. While browser hardening can reduce fingerprinting effectiveness, complete anonymity is not achievable, especially on rare operating systems such as Kali Linux.
