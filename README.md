# Awesome-Workforce-Device-Trust

# Similar Projects to Workforce Device Trust Platforms

**Workforce Device Trust Platforms** continuously assess the security posture and compliance of employee devices (laptops, mobiles, etc.) and use that signal for zero-trust access decisions, conditional access, and endpoint management. Leading commercial solutions include Kolide, Kandji, JumpCloud Device Trust, Microsoft Intune, Cisco Duo Device Trust, Jamf Protect, Workspace ONE, Uptycs Device Trust, Tanium, and Scalefusion.

Below is a **curated list** of notable platforms and their open-source equivalents. The open-source ecosystem is particularly strong in this space thanks to osquery-based visibility and modern open MDM platforms.

## 🏢 SaaS / Hosted Platforms

- **[Kolide](https://www.kolide.com/)** — Device trust and compliance platform focused on user-friendly posture checks and remediation guidance (especially strong on macOS/Linux visibility).
- **[Kandji](https://www.kandji.io/)** — Modern Apple-focused device management and security platform.
- **[JumpCloud Device Trust](https://jumpcloud.com/)**, **[Microsoft Intune](https://www.microsoft.com/en-us/security/business/microsoft-intune)**, **[Cisco Duo Device Trust](https://duo.com/)**, **[Jamf Protect](https://www.jamf.com/)**, **[Workspace ONE](https://www.omnissa.com/)**, **[Uptycs](https://www.uptycs.com/)**, **[Tanium](https://www.tanium.com/)**, **[Scalefusion](https://scalefusion.com/)** — Enterprise device management, endpoint security, and device-trust / conditional-access solutions.

## 🔓 Open-Source Software

### Leading Open-Source Device Management & Posture
- **[Fleet](https://github.com/fleetdm/fleet)** (FleetDM) — The premier open-source device management and device-trust platform. Built on osquery, it provides real-time visibility, policy enforcement, vulnerability detection, MDM capabilities (macOS, Windows, Linux, and more), GitOps workflows, and strong support for zero-trust posture assessment. Self-hostable and highly transparent.
- **[osquery](https://github.com/osquery/osquery)** — Foundational open-source endpoint instrumentation framework that exposes operating-system data as a high-performance relational database. Powers Fleet and many commercial device-trust solutions; excellent for custom posture queries and compliance checks.

### Additional Open-Source MDM / Endpoint Tools
- Emerging and community open-source MDM projects that support multi-platform enrollment, configuration profiles, and basic device management (including projects aiming for full multi-OS coverage).
- Open-source RMM (Remote Monitoring and Management) platforms such as MeshCentral and TacticalRMM that provide visibility, scripting, and remote management capabilities useful in device-trust workflows.

### Zero-Trust Access with Device Posture
- **Teleport**, **OpenZiti**, **Pomerium**, and similar open-source zero-trust access tools that can incorporate device posture checks as part of access decisions.
- Policy engines (e.g., Open Policy Agent) that can evaluate device signals alongside identity for fine-grained authorization.

### Typical Open-Source Approach
1. **Visibility & telemetry** — osquery agents collecting rich endpoint data
2. **Control plane** — Fleet for querying, policy, MDM actions, and compliance reporting
3. **Access enforcement** — Integrate posture results into an identity-aware proxy or zero-trust gateway (Teleport, Pomerium, etc.)
4. **Remediation** — Scripts, profiles, and GitOps-driven configuration management
5. **Reporting & audit** — Export to SIEM or data lake for continuous monitoring

This stack delivers transparent, auditable device trust without proprietary agent lock-in and works across mixed OS fleets.

---

**How to contribute**  
Fork this repository, add a new project (with link + short description + category), and open a pull request.  
Prefer actively maintained open-source projects related to device trust, endpoint posture, MDM, osquery management, or zero-trust device assessment.

**License**  
This list is public domain / CC0. Feel free to copy into your own awesome list or README.

Star the projects you find useful — open device-trust tools help organizations verify endpoints without black boxes! 🔐
