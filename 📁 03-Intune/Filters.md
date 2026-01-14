# Intune Filters – AlphaTravel

## Purpose
Filters are used to narrow device targeting inside groups
without creating additional device groups.

## Filters in use

### FLT-Windows-Corporate
- OS: Windows
- Ownership: Corporate

Rule:
(device.deviceOSType -eq "Windows") and
(device.deviceOwnership -eq "Corporate")

---

### FLT-macOS-Developers
- OS: macOS
- Used with: UG-Developers

Rule:
(device.deviceOSType -eq "MacMDM")

---

### FLT-Android-Sales
- OS: Android
- Ownership: Corporate
- Used with: UG-Sales

Rule:
(device.deviceOSType -eq "Android") and
(device.deviceOwnership -eq "Corporate")
