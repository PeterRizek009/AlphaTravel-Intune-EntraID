
flowchart TB

%% =====================
%% Nodes
%% =====================
DEVICES[AlphaTravel<br/>Corporate Devices]

WIN[Windows Devices<br/>
------------------<br/>
DG-Windows-All]

MAC[macOS Devices (Developers)<br/>
------------------<br/>
DG-macOS-Developers]

AND[Android Devices (Sales)<br/>
------------------<br/>
DG-Android-Sales]

%% =====================
%% Relationships
%% =====================
DEVICES --> WIN
DEVICES --> MAC
DEVICES --> AND

%% =====================
%% Styles
%% =====================
classDef company fill:#1f2937,color:#ffffff,stroke:#60a5fa,stroke-width:2px;
classDef windows fill:#1e3a8a,color:#ffffff,stroke:#93c5fd,stroke-width:2px;
classDef macos fill:#065f46,color:#ffffff,stroke:#6ee7b7,stroke-width:2px;
classDef android fill:#3f6212,color:#ffffff,stroke:#bef264,stroke-width:2px;

class DEVICES company
class WIN windows
class MAC macos
class AND android
