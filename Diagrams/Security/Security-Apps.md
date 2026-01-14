
flowchart TB

APPSEC["AlphaTravel<br/>Apps & Data Security"]

APPTYPES["App Types<br/>
Microsoft 365 (Outlook / Teams / Edge)<br/>
CRM Web / App<br/>
Dev Tools (VS Code / GitHub)<br/>
Optional Apps (Zoom / WhatsApp Business)"]

CONTROLS["Security Controls<br/>
App Protection (MAM)<br/>
App Configuration Policies<br/>
Data Loss Prevention (DLP)<br/>
Conditional Access for Apps<br/>
Approved Apps Only"]

RULES["Example App Rules<br/>
Require PIN for corporate apps<br/>
Block copy & paste to personal apps<br/>
Block backup to personal cloud<br/>
Require approved client apps"]

APPSEC --> APPTYPES
APPSEC --> CONTROLS
APPSEC --> RULES

classDef header fill:#1f2937,color:#ffffff,stroke:#60a5fa,stroke-width:2px;
classDef apps fill:#1e3a8a,color:#ffffff,stroke:#93c5fd,stroke-width:2px;
classDef box fill:#111827,color:#ffffff,stroke:#9ca3af,stroke-width:2px;

class APPSEC header
class APPTYPES apps
class CONTROLS,RULES box
