```mermaid
flowchart TB

COMPANY[AlphaTravel<br/>Corporate Users]

HO[Head Office Users<br/>
------------------<br/>
UG-HO-Management<br/>
UG-HO-IT<br/>
UG-HO-Finance<br/>
UG-HO-Operations<br/>
UG-HO-Developers]

BR1[Branch 1 Users<br/>
------------------<br/>
UG-BR1-Sales<br/>
UG-BR1-Manager]

BR2[Branch 2 Users<br/>
------------------<br/>
UG-BR2-Sales<br/>
UG-BR2-Manager]

BR3[Branch 3 Users<br/>
------------------<br/>
UG-BR3-Sales<br/>
UG-BR3-Manager]

BR4[Branch 4 Users<br/>
------------------<br/>
UG-BR4-Sales<br/>
UG-BR4-Manager]

BR5[Branch 5 Users<br/>
------------------<br/>
UG-BR5-Sales<br/>
UG-BR5-Manager]

COMPANY --> HO
COMPANY --> BR1
COMPANY --> BR2
COMPANY --> BR3
COMPANY --> BR4
COMPANY --> BR5
