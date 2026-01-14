```mermaid
flowchart TB

COMPANY[AlphaTravel<br/>Corporate Users]

HO[Head Office Users<br/>
------------------<br/>
UG-Management<br/>
UG-IT<br/>
UG-Finance<br/>
UG-Operations<br/>
UG-Developers]

SALES[Sales Users<br/>
------------------<br/>
UG-Sales]

SM[Sales Managers<br/>
------------------<br/>
UG-Sales-Managers]

COMPANY --> HO
COMPANY --> SALES
COMPANY --> SM

