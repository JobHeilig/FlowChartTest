# FlowChartTest
```mermaid
flowchart TD

start((enter word beschikbaar)) --> A(drukt op enter)
A --> B(Mechanic start)
B --> C(Bom spawnt en valt naar beneden met een geluid en een smoke effect dat het achterlaat)
C --> D(Bom valt op het slagveld)
D --> E(Bom ontploft)
E --> F(Explosie gaat over het hele slagveld)
F --> G{Staan er vijanden op het slagveld?}
G -- Ja --> H[Iedereen is uitgeroeid. Jouw fort heeft zelf ook wat schade opgelopen]
G -- Nee --> I[You fucked up! Wapen verspild en fort heeft schade opgelopen voor niets!]
G -- Nee EN je fort heeft niet genoeg health meer -->K[Je fort heeft schade opgelopen tot het doodging. Je hebt het spel verloren]
H --> J((Mechanic voorbij! Wacht ongeveer 3 waves zonder de bom))
I --> J((Mechanic voorbij! Wacht ongeveer 3 waves zonder de bom))
J -- Wacht 3 waves --> start
