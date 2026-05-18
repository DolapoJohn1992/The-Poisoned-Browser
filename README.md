# 🛠️ THE POISONED BROWSER: CLIENT-SIDE EXPLOITATION LAB
**Cybersecurity Portfolio Artifact | Weaponized Payload Logs & Defenses**

---

## 📑 PROJECT OVERVIEW
This laboratory exercises advanced client-side exploitation methodologies within a dedicated, isolated Ubuntu workstation targeting the vulnerable **"Titan Social Network"** sandbox. The objective was to identify input-validation flaws, weaponize cross-site scripting vectors to hijack active session metrics, forge unauthorized state-changing financial interactions, and document enterprise mitigation requirements.

---

## 🎯 LABORATORY OBJECTIVES
* **Identify and Exploit Reflected XSS:** Intercept and manipulate Document Object Model (DOM) rendering via unvalidated search query strings.
* **Weaponize Stored XSS for Session Hijacking:** Inject dynamic JavaScript arrays into persistent storage assets to exfiltrate administrative active tokens (`document.cookie`).
* **Craft Cross-Site Request Forgery (CSRF) Links:** Reverse-engineer transaction application flows to force unauthenticated financial actions.
* **Define Enterprise-Grade Protections:** Outline precise developer mitigation practices to secure frontend architectures.

---

## 🔬 TECHNICAL ARTIFACTS & EXPLOITATION MECHANICS

### 🔹 Phase 1: Reflected XSS (The Reflection)
* **Vulnerable Parameter:** User Search Field Layer (`/search?q=`)
* **Exploitation Script:** ```html
  <script>alert('XSS')</script>
