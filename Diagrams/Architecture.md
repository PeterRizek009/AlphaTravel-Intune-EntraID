```mermaid
flowchart TB
HO_USERS[Head Office Users]
BR1[Branch 1 Sales]
BR2[Branch 2 Sales]
BR3[Branch 3 Sales]
BR4[Branch 4 Sales]
BR5[Branch 5 Sales]

ENTRA[Microsoft Entra ID]
INTUNE[Microsoft Intune]

WIN[Windows Devices]
MAC[macOS Devices - Developers]
AND[Android Devices - Sales]

CA[Conditional Access]
COMP[Compliance Policies]
MDE[Defender for Endpoint]

HO_USERS --> ENTRA
BR1 --> ENTRA
BR2 --> ENTRA
BR3 --> ENTRA
BR4 --> ENTRA
BR5 --> ENTRA

ENTRA --> CA
ENTRA --> INTUNE

INTUNE --> WIN
INTUNE --> MAC
INTUNE --> AND

INTUNE --> COMP
INTUNE --> MDE

CA --> WIN
CA --> MAC
CA --> AND
