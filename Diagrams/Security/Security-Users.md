```mermaid
flowchart TB

USERS["AlphaTravel<br/>Users Security"]

TYPES["User Types<br/>
- Standard Users<br/>
- Sales<br/>
- Sales Managers<br/>
- Developers<br/>
- IT Admins"]

CONTROLS["Security Controls<br/>
- MFA<br/>
- SSPR<br/>
- RBAC Roles<br/>
- Conditional Access<br/>
- Sign-in Risk Policies"]

POLICIES["Example Policies<br/>
- MFA for all users<br/>
- Require compliant device for Managers & Finance<br/>
- Block legacy authentication<br/>
- Block high-risk sign-ins"]

USERS --> TYPES
USERS --> CONTROLS
USERS --> POLICIES

classDef header fill:#1f2937,color:#ffffff,stroke:#60a5fa,stroke-width:2px;
classDef box fill:#111827,color:#ffffff,stroke:#9ca3af,stroke-width:2px;

class USERS header
class TYPES,CONTROLS,POLICIES box
