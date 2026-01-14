# Entra ID – Dynamic Groups Design

## Branch-based user groups
- DG-HO-Users
- DG-BR1-Users
- DG-BR2-Users
- DG-BR3-Users
- DG-BR4-Users
- DG-BR5-Users

### Example Rule (Branch1)
(user.officeLocation -eq "BR1")

## Role / Department groups
- DG-Sales
- DG-Branch-Managers
- DG-Developers
- DG-IT
- DG-Finance
- DG-Operations

### Example Rules
Sales:
(user.department -eq "Sales")

Branch Managers:
(user.jobTitle -contains "Branch Manager")

Developers:
(user.department -eq "Developers")

## Device groups
- DG-Windows-All
- DG-Windows-Branches
- DG-macOS-Developers
- DG-Android-Corp

### Device Rule Examples
Windows all:
(device.deviceOSType -eq "Windows")

macOS:
(device.deviceOSType -eq "MacMDM")

Android:
(device.deviceOSType -eq "Android")
