# Entra ID – Conditional Access Policies (Zero Trust)

## CA-01: Require MFA for all users
- Users: All users
- Cloud apps: All cloud apps
- Grant: Require multifactor authentication
- Exclusions: Break-glass account(s) only

## CA-02: Block Legacy Authentication
- Users: All users
- Client apps: Other clients + legacy auth
- Grant: Block access

## CA-03: Require compliant device for Managers + Finance
- Users: DG-Branch-Managers, DG-Finance, DG-Management
- Cloud apps: All cloud apps (or Office 365)
- Grant: Require device to be marked as compliant

## CA-04: Sales access allowed only from enrolled Android/Windows
- Users: DG-Sales
- Grant: Require device to be marked as compliant
- Additional control: Require approved client app (mobile)

## CA-05: macOS allowed only for Developers
- Users: All users
- Conditions: Device platform includes macOS
- Exclude: DG-Developers
- Grant: Block access

## CA-06: Block access from high-risk sign-ins (Optional)
- Users: All users
- Conditions: Sign-in risk = High
- Grant: Block access

## Notes
- Maintain 1–2 break-glass accounts with strong protections.
- Keep CA policies in report-only first, then enforce.
