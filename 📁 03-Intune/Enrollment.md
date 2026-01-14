# Intune – Enrollment Plan

## Windows (All non-dev users)
- Join type: Entra ID Join
- Automatic MDM enrollment: Enabled
- Autopilot: Used for all new Windows devices
- Naming: AT-WIN-%SERIAL%

Assignments
- Autopilot profile -> DG-Windows-All
- Enrollment restrictions -> allow Windows + block personal devices (optional)

## macOS (Developers - HO)
- Enrollment: Company Portal (Apple MDM)
- Device group: DG-Developers + DG-macOS-Developers
- Naming: AT-MAC-%SERIAL% (documented standard)

## Android (Sales devices)
- Ownership: Corporate-owned, fully managed
- Enrollment: Android Enterprise Fully Managed
- Naming: AT-AND-%SERIAL%
- Block BYOD for Sales (policy decision)
