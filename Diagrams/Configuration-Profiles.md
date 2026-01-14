```mermaid
flowchart TB

INTUNE["Microsoft Intune"]

PROFILES["Configuration Profiles"]

WIN_PROF["Windows Profiles
- Security Baseline
- OneDrive KFM
- Windows Update Rings"]

MAC_PROF["macOS Profiles
- FileVault
- Firewall
- Software Updates"]

AND_PROF["Android Profiles
- Screen Lock
- Encryption
- App Restrictions"]

UG["User Groups
UG-Sales
UG-Developers
UG-IT"]

INTUNE --> PROFILES

PROFILES --> WIN_PROF
PROFILES --> MAC_PROF
PROFILES --> AND_PROF

WIN_PROF --> UG
MAC_PROF --> UG
AND_PROF --> UG

classDef intune fill:#1f2937,color:#ffffff,stroke:#60a5fa,stroke-width:2px;
classDef profiles fill:#0f766e,color:#ffffff,stroke:#5eead4,stroke-width:2px;
classDef windows fill:#1e3a8a,color:#ffffff,stroke:#93c5fd,stroke-width:2px;
classDef macos fill:#065f46,color:#ffffff,stroke:#6ee7b7,stroke-width:2px;
classDef android fill:#3f6212,color:#ffffff,stroke:#bef264,stroke-width:2px;
classDef groups fill:#7c2d12,color:#ffffff,stroke:#fdba74,stroke-width:2px;

class INTUNE intune
class PROFILES profiles
class WIN_PROF windows
class MAC_PROF macos
class AND_PROF android
class UG groups

