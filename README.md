<div align="center">

# 🛡️ WhiteHats Club — Recruitment Task

![Cybersecurity](https://img.shields.io/badge/Focus-Cybersecurity%20%26%20Ethical%20Hacking-0A66C2?style=for-the-badge&logo=hackthebox&logoColor=white)
![Reg No](https://img.shields.io/badge/Reg%20No-26BIT0259-00C853?style=for-the-badge)
![Status](https://img.shields.io/badge/Applicant-Soham%20Yadav-8A2BE2?style=for-the-badge)

</div>

---

## 👨‍💻 1. Applicant Profile

| Field | Details |
| :--- | :--- |
| **Name** | **Soham Yadav** |
| **Registration No.** | **`26BIT0259`** |
| **GitHub** | [@soham007-y](https://github.com/soham007-y) |
| **Interests** | Ethical Hacking, Network Security, CTFs, Vulnerability Research |

```bash
$ whoami
soham_yadav (26BIT0259) — Aspiring Security Researcher & WhiteHat
```

---

## 🚀 2. Why I Want to Join WhiteHats

> *"To beat a hacker, you need to think like one—and build a community that defends together."*

I want to join **WhiteHats** because I am deeply passionate about **cybersecurity, ethical hacking, and understanding how modern systems operate under the hood**. Rather than just studying theory, I want to dive into real-world offensive and defensive security challenges.

Joining **WhiteHats** will allow me to:
- 🚩 **Compete in CTFs (Capture The Flag):** Sharpen my problem-solving skills across cryptography, web exploitation, reverse engineering, and forensics.
- 🤝 **Collaborate & Learn with Peers:** Surround myself with driven security enthusiasts, share knowledge, and learn from experienced seniors.
- 🔍 **Gain Hands-On Security Experience:** Explore penetration testing, vulnerability assessment, and secure coding practices through workshops and live projects.
- 🌐 **Contribute to Cyber Awareness:** Help foster a strong security-first culture across campus.

---

## 📰 3. Recent Cybersecurity Incident I Read About

### 🎯 The XZ Utils Supply Chain Backdoor (`CVE-2024-3094`)

| Attribute | Overview |
| :--- | :--- |
| **Target** | `XZ Utils` (v5.6.0 & v5.6.1) — Linux lossless data compression library (`liblzma`) |
| **Attack Type** | Multi-year Open-Source Supply Chain & Social Engineering Attack |
| **Severity** | **CVSS 10.0 (Critical)** — Pre-authentication Remote Code Execution (RCE) as `root` |
| **Threat Actor** | Alias **`Jia Tan`** |

#### 🧠 What Happened?
1. **Long-Con Social Engineering:** Over nearly two years, an attacker using the alias *Jia Tan* made legitimate contributions to the **XZ Utils** repository and used sockpuppet accounts to pressure the original sole maintainer into granting maintainer access.
2. **Stealthy Payload Injection:** In early 2024, *Jia Tan* hid obfuscated malicious object files inside innocent-looking binary test files in the release tarballs for versions `5.6.0` and `5.6.1`.
3. **Hooking into OpenSSH (`sshd`):** On Linux distributions using `systemd`, the `sshd` binary indirectly loads `liblzma`. The backdoor used `glibc` `IFUNC` resolvers during the build process to hijack `RSA_public_decrypt`, allowing anyone holding a specific **Ed448 private key** to bypass SSH authentication and execute arbitrary commands as `root`.
4. **Accidental Discovery:** Microsoft engineer **Andres Freund** caught the backdoor before it reached stable production releases after noticing that failed SSH logins were taking ~500ms longer than usual and consuming abnormal CPU cycles.

#### 💡 Key Takeaway
> [!IMPORTANT]
> Even the most battle-tested cryptographic protocols like **SSH** can be compromised through upstream dependencies. This incident proved that **open-source supply chain security** and **proactive performance/anomaly monitoring** are critical pillars of modern cybersecurity.

---

<div align="center">
  <sub>Crafted with 💻 & 🔒 by <b>Soham Yadav (26BIT0259)</b> for <b>WhiteHats</b></sub>
</div>
