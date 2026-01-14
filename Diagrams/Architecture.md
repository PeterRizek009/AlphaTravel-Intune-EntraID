flowchart TB

%% =====================
%% USERS
%% =====================
USERS[Corporate Users - AlphaTravel]

HO[Head Office Users]
BR[Branch Sales Users]

USERS --> HO
USERS --> BR

%% =====================
%% IDENTITY
%% =====================
ENTRA[Microsoft Entra ID]

HO --> ENTRA
BR --> ENTRA

%% =====================
%% DEVICES
%% =====================
CORP_DEV[Corporate Devices]

WIN[Windows Devices]
MAC[macOS Devices - Developers]
AND[Android Devices - Sales]

CORP_DEV --> WIN
CORP_DEV --> MAC
CORP_DEV --> AND

%% =====================
%% MANAGEMENT
%% =====================
INTUNE[Microsoft Intune]

WIN --> INTUNE
MAC --> INTUNE
AND --> INTUNE

%% =====================
%% SECURITY
%% =====================
CA[Conditional Access]
COMP[Compliance Policies]
DEF[Defender for Endpoint]

ENTRA --> CA
INTUNE --> COMP
INTUNE --> DEF

CA --> WIN
CA --> MAC
CA --> AND

