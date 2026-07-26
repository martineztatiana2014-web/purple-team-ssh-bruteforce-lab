nano README.md
# Purple Team Project: SSH Brute-Force Attack & Detection

This project demonstrates a full Purple Team workflow by simulating an SSH brute-force attack, detecting malicious authentication attempts, and applying defensive countermeasures. It showcases Red Team attack execution, Blue Team log analysis, and Purple Team reporting.

---

## 🔴 Red Team: Attack Simulation

**Objective:** Generate repeated failed SSH login attempts for detection.

**Tool Used:** Hydra  
**Command Executed:**

**Outcome:** Multiple failed SSH login attempts were generated and logged in `/var/log/auth.log`.

---

## 🔵 Blue Team: Detection & Analysis

**Log File Monitored:**  
`/var/log/auth.log`

**Indicators Observed:**
- Repeated failed SSH login attempts  
- Same source IP  
- Rapid authentication failures  
- Clear brute-force pattern

**Commands Used:**

---

## 🛡️ Blue Team: Response Actions

**Defensive Measures Implemented:**
- Blocked attacking IP using UFW  
- Enabled SSH rate limiting  
- Recommended disabling password authentication  
- Reviewed system logs for additional anomalies

**Commands Used:**

---

## 🟣 Purple Team: Combined Analysis

This section maps the Red Team attack to Blue Team detection and response.

**Key Takeaways:**
- SSH brute-force attacks are easily detectable through log monitoring.
- Rate limiting and firewall rules significantly reduce attack success.
- Password authentication should be replaced with SSH keys.
- Purple Team collaboration strengthens both offensive and defensive capabilities.

---

## 📁 Repository Structure


---

## 🎯 Skills Demonstrated

- Red Team attack simulation  
- Blue Team log analysis  
- Incident response  
- Purple Team methodology  
- Linux security hardening  
- Git & GitHub workflow  
- Documentation and reporting  
