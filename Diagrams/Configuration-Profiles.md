flowchart TB

INTUNE["Microsoft Intune"]

PROFILES["Configuration Profiles"]

WIN_PROF["Windows Profiles\n- Security Baseline\n- OneDrive KFM\n- Windows Update Rings"]

MAC_PROF["macOS Profiles\n- FileVault\n- Firewall\n- Software Updates"]

AND_PROF["Android Profiles\n- Screen Lock\n- Encryption\n- App Restrictions"]

UG["User Groups\nUG-Sales\nUG-Developers\nUG-IT"]

FLT["Filters\nFLT-Windows-Corporate\nFLT-macOS-Developers\nFLT-Android-Sales"]

DEV["Target Devices"]

INTUNE --> PROFILES

PROFILES --> WIN_PROF
PROFILES --> MAC_PROF
PROFILES --> AND_PROF

WIN_PROF --> UG
MAC_PROF --> UG
AND_PROF --> UG

UG --> FLT
FLT --> DEV

classDef intune fill:#1f2937,color:#ffffff,stroke:#60a5fa,stroke-width:2px;
classDef profiles fill:#0f766e,color:#ffffff,stroke:#5eead4,stroke-width:2px;
classDef windows fill:#1e3a8a,color:#ffffff,stroke:#93c5fd,stroke-width:2px;
classDef macos fill:#065f46,color:#ffffff,stroke:#6ee7b7,stroke-width:2px;
classDef android fill:#3f6212,color:#ffffff,stroke:#bef264,stroke-width:2px;
classDef groups fill:#7c2d12,color:#ffffff,stroke:#fdba74,stroke-width:2px;
classDef filters fill:#4c1d95,color:#ffffff,stroke:#c4b5fd,stroke-width:2px;
classDef devices fill:#111827,color:#ffffff,stroke:#9ca3af,stroke-width:2px;

class INTUNE intune
class PROFILES profiles
class WIN_PROF windows
class MAC_PROF macos
class AND_PROF android
class UG groups
class FLT filters
class DEV devices
