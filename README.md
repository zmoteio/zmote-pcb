# zmote-pcb
schematics,design and gerber files for the zmote widget

[schematics](zmote.pdf)

[Gerbers](gerbers/)

[zmote PCBs](http://dirtypcbs.com/view.php?share=9978&accesskey=257368fbcf180a8e00e58f2eab851304)

# Setup for making changes to the PCB
* Install ki-cad from http://kicad-pcb.org/download/
* Get Ki-cad component library for ESP modules
  * git clone https://github.com/klarsys/kicad-ESP8266.git
* Get this repository
  * git clone https://github.com/zmoteio/zmote-pcb.git
* Update ki-cad component library path
  * Add kicad-ESP8266/ESP8266 under ki-cad->Eeschema->Preferences
* Update ki-cad component footprint path under under ki-cad->Pcbnew->Preferences->Footprint Libraries Manager
  * Add ESP8266 with path kicad-ESP8266/ESP8266.pretty
  * Add zmote-custom with path zmote-custom.pretty
* make changes to schematics and PCB using schematic editor and PCB editor
* ki-cad setup for dumping gerber and drilling files
  * [kicad-settings-drill.png](gerbers/kicad-settings-drill.png)
  * [kicad-settings-gerbergen.png](gerbers/kicad-settings-gerbergen.png)
