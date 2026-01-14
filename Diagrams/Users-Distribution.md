```mermaid
flowchart TB

%% =====================
%% Nodes
%% =====================
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

%% =====================
%% Relationships
%% =====================
COMPANY --> HO
COMPANY --> SALES
COMPANY --> SM

%% =====================
%% Styles
%% =====================
classDef company fill:#1f2937,color:#ffffff,stroke:#60a5fa,stroke-width:2px;
classDef headoffice fill:#0f766e,color:#ffffff,stroke:#5eead4,stroke-width:2px;
classDef sales fill:#7c2d12,color:#ffffff,stroke:#fdba74,stroke-width:2px;
classDef managers fill:#4c1d95,color:#ffffff,stroke:#c4b5fd,stroke-width:2px;

class COMPANY company
class HO headoffice
class SALES sales
class SM managers


