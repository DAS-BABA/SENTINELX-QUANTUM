# 🛡️ SentinelX Quantum Guardian
### AI-Powered Predictive Privileged Access & Insider Threat Prevention Platform
**FinSpark '26 – Banking Cybersecurity Innovation Hackathon Project**  
*Developed with ❤️ by Team **Har Har Mahadev***

---

## ⚡ Executive Summary
Traditional Security Information and Event Management (SIEM) systems and Privileged Access Management (PAM) architectures are **fundamentally reactive**. They record, parse, and alert on incidents *after* credentials have been compromised, databases wiped, or SWIFT transaction files exfiltrated. 

**SentinelX Quantum Guardian** shifts the security paradigm from reactive mitigation to **active inline prevention**. It establishes a **Behavioural Digital Twin** profile for system administrators, continuously measuring motor-cognitive dynamics (keystroke flight intervals, mouse velocity jitters) and access patterns. The platform evaluates risk using a **Dynamic Trust Decay Engine** and applies automated inline controls—such as FIDO2 step-up MFA, terminal locking, and IP blacklisting—before queries execute. 

All audit trails, configuration states, and incident logs are cryptographically sealed in an immutable **Quantum Vault** utilizing FIPS 203/204 post-quantum standards (Kyber & Dilithium), guaranteeing forensic integrity against future quantum decryption threats.

---

## 🚀 Key Innovation Pillars

```
+-----------------------------------------------------------------------------------+
|                              SENTINELX SECURITY CORE                              |
+--------------------------+---------------------------+----------------------------+
|  1. BEHAVIOURAL TWIN     |  2. TRUST DECAY ENGINE    |  3. QUANTUM-SAFE VAULT     |
|  Continuous profiling of |  Dynamic risk attribution |  Forensic logs sealed with |
|  keystrokes and mouse    |  replaces static rules.   |  Dilithium & Kyber keys    |
|  biometric velocities.   |  Decays on anomalies.     |  against future threats.   |
+--------------------------+---------------------------+----------------------------+
```

1. **Biometric DNA Mapping (Cognitive Telemetry)**
   - Establishes a non-spoofable behavioral profile based on keystroke rhythm and mouse movement curves.
   - Detects remote session hijacking even when the attacker is using valid administrative passwords and tokens.

2. **Real-Time Interactive Floor Plan Map**
   - A visual, spatial monitoring blueprint mapping physical desks, Data Center racks, and Gateway Closets.
   - Live network packet flows animate normal (green) vs. anomalous data exfiltration (red) streams.
   - Provides direct administrative overrides: Lock Terminals, Sever Active Directory Sessions, Quarantine Database Racks, and Blacklist Attacker IP Addresses with a single click.

3. **Decoy Shell & Command Simulator**
   - Intercepts privileged command calls (e.g., database deletions) and evaluates the potential business impact (financial cost, regulatory fines, expected downtime).
   - Unsafe commands are blocked inline, and administrative sessions are isolated without impacting production workloads.

4. **Explainable AI (XAI) Attribution**
   - Risk scoring models expose exactly *why* an alert was generated (e.g., 92% Intent due to unusual MAC signature + 02:13 AM login + database dump size exceeding 30-day baseline by 4,200%).

---

## 🛠️ Technology Stack
* **Core Interface**: React 18 + TypeScript + Vite
* **Design & Styling**: Vanilla CSS + Tailwind CSS v3 (Glassmorphic dark-neon cyberpunk theme)
* **Real-time Graphics**: HTML5 Canvas (glowing background particles) + SVG (interactive office blueprint layouts)
* **Data Visualization**: Recharts (biometric dynamics, trend charts)
* **Iconography**: Lucide React
* **Presentation Deck**: Standalone Reveal.js engine (responsive, keyboard-navigated, embedded diagrams)

---

## 📂 Project Architecture & Code Map
```text
├── presentation.html         # Reveal.js 21-slide pitch deck (16:9 widescreen layout)
├── index.html                # Main mount page template
├── tailwind.config.js        # Custom cyber-neon color configuration
├── package.json              # Compilation scripts and dependencies
├── src/
│   ├── main.tsx              # React mounting root
│   ├── App.tsx               # Main layout router and global emergency lockdown overlay
│   ├── index.css             # Base styles, scrollbars, scanlines, and glow keyframes
│   ├── components/
│   │   ├── Sidebar.tsx       # Navigation bar and global core shield status indicator
│   │   └── DemoController.tsx# Interactive panel triggering 6-step flight path demo
│   ├── context/
│   │   └── DemoContext.tsx   # Global state machine containing data indices and incident updates
│   ├── utils/
│   │   └── mockData.ts       # Mock database models (employees, branch logs, Neo4j graphs)
│   └── screens/
│       ├── OverviewScreen.tsx    # Screen 1: Executive KPI counters, risk scores, and trend charts
│       ├── HeatmapScreen.tsx     # Screen 2: Risk heatmaps of Indian banking branch nodes
│       ├── DigitalTwinScreen.tsx # Screen 3: Floor Plan Blueprint & Biometric DNA charts
│       ├── ThreatFeedScreen.tsx  # Screen 4: Real-time incident logs and explainable AI alerts
│       ├── SimulatorScreen.tsx   # Screen 5: Privilege Command Terminal & Impact Simulator
│       ├── QuantumVaultScreen.tsx# Screen 6: FIPS PQC Audit Log Archive (Kyber/Dilithium)
│       ├── ThreatGraphScreen.tsx # Screen 7: Relational Asset Connection Matrix
│       └── SOCCommandScreen.tsx  # Screen 8: SOC Command War Room (AI Analyst Copilot)
```

---

## 🖥️ Screen-by-Screen Features

### 1. Executive Security Console (`OverviewScreen.tsx`)
* Displays key risk indicators (KPIs) including active threats, average trust index score trends, and Quantum Vault verification statuses.
* Renders a 7-day Trust DNA trend chart plotting Ramesh Patel vs. Rohan Gupta.
* Highlights risk distribution metrics by branch location (Mumbai HQ, Bangalore, Chennai, etc.).

### 2. Geographical Branch Heatmap (`HeatmapScreen.tsx`)
* Maps branch coordinates across India with interactive pulse rings.
* Displays local risk score indices, active terminal count, and database replication statuses.

### 3. Behavioural Floor Plan & DNA Telemetry (`DigitalTwinScreen.tsx`)
* **Live Office Blueprint**: Integrates a vector map of desks, servers, and routers. Green packet streams animate active traffic; red packet streams animate data exfiltration paths to rogue MacBooks outside the office WAN perimeter.
* **Diagnostics Node Inspector**: Click on any map asset to execute manual security controls:
  - *Desk Node*: Challenge MFA, Scan Biometrics, Lock Terminal, or Sever active session tokens.
  - *Data Center Server Node*: Run database integrity checks (table scans against SHA-256 keys) or quarantine the SQL server.
  - *Edge Router Gateway Node*: Instantly blacklist rogue attacker IP `192.168.4.15`, severing exfiltration packets.
  - *Rogue Node*: Inspect exfiltration logs and connection ports.
* **DNA Telemetry Tab**: Displays mouse velocity jitter maps, typing interval dynamics charts, and historical timeline logs.

### 4. Live Threat Feed (`ThreatFeedScreen.tsx`)
* Real-time stream of audit logs with explainable AI panels mapping telemetry attributes to risk weights.

### 5. Privilege Command Simulator (`SimulatorScreen.tsx`)
* Shell terminal allowing administrators to test destructive SQL queries (e.g. `DROP TABLE CUSTOMER`). Intercepts command execution, calculates financial business loss, and locks credentials.

### 6. Quantum Vault Archive (`QuantumVaultScreen.tsx`)
* Archive of cryptographically sealed audit records signed with CRYSTALS-Dilithium signatures.

### 7. Insider Threat Graph (`ThreatGraphScreen.tsx`)
* Relational node graph mapping lateral connections between employees, laptops, Active Directory hosts, and production databases to identify credential-sharing anomalies.

### 8. SOC Command War Room (`SOCCommandScreen.tsx`)
* A command deck featuring the global risk index level, active threat lists, global lockdown toggle overrides, and the SentinelX AI Security Analyst chat.

---

## 🛄 Running the Platform Locally

### Prerequisites
Make sure you have [Node.js](https://nodejs.org/) (v18+) installed.

### 1. Install Dependencies
```bash
npm install
```

### 2. Run Local Development Server
```bash
npm run dev
```
Open your browser and navigate to the address shown in the terminal (typically `http://localhost:5173` or `http://localhost:5174`).

### 3. Compile Production Bundle
```bash
npm run build
```

---

## 📽️ Interactive Demo Flight Path
To demonstrate the platform's response to an active administrative breach, click the **Demo Flight Controller** in the bottom-right corner of the screen:

1. **Step 1: Baseline Normal**: Admin Ramesh Patel logs in normally from his corporate Windows laptop. (Trust DNA: 95%, secure).
2. **Step 2: Device Mismatch**: Ramesh logs in at 02:13 AM from an unregistered MacBook. (Trust decays to 85%, warning triggers).
3. **Step 3: Massive Data Export**: Ramesh's session downloads a 4.8GB customer ledger. (Trust decays to 65%, exfiltration stream begins).
4. **Step 4: Destructive Command**: The session executes `DROP TABLE CUSTOMER`. SentinelX simulator intercepts, blocks the query, and logs a potential loss of **₹6.8 Crore**. (Trust decays to 35%).
5. **Step 5: AI Insider Prediction**: AI Threat Predictor correlates anomalies and forecasts a **92% malicious behavior intent**. (Warning alerts trigger).
6. **Step 6: Adaptive Mitigation**: System revokes all active session tokens, suspends AD credentials, blacklists the rogue MAC IP, and seals audit logs. (Ramesh's desk locks down on the Floor Plan, threat is neutralized).

*Note: You can bypass the automatic steps and execute manual mitigations (like clicking the router gateway to block the attacker IP or severing Ramesh's session) directly on the **Floor Plan Map**!*

---

## 📽️ Reveal.js Pitch Deck
To view the pitch deck slides:
1. Open the file `presentation.html` in any web browser.
2. Use **Left / Right arrow keys** or **Space** to navigate slides.
3. Hover over the architectural diagram nodes on **Slide 14** to inspect components.
4. Click on the carousel tabs on **Slide 15** to browse screenshots of the live system and watch the simulated command mitigation video.

---

### Developed for FinSpark '26
**Team Har Har Mahadev**  
* Saumil Prajapati  
* Ishita Singh  
* Sachi Parikh  
* Pratham Solanki  
