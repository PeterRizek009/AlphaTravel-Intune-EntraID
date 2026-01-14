flowchart TB

USERS["AlphaTravel\nUsers Security"]

TYPES["User Types\n- Standard Users\n- Sales\n- Sales Managers\n- Developers\n- IT Admins"]

CONTROLS["Security Controls\n- MFA\n- SSPR\n- RBAC Roles\n- Conditional Access\n- Sign-in Risk Policies"]

POLICIES["Example Policies\n- MFA for all\n- Require compliant device for Managers/Finance\n- Block legacy auth\n- Block high-risk sign-ins"]

USERS --> TYPES
USERS --> CONTROLS
USERS --> POLICIES

classDef header fill:#1f2937,color:#ffffff,stroke:#60a5fa,stroke-width:2px;
classDef box fill:#111827,color:#ffffff,stroke:#9ca3af,stroke-width:2px;

class USERS header
class TYPES,CONTROLS,POLICIES box
