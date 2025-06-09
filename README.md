# Acorn Archimedes ARM6 (ARM610/ARM710) processor card

June 2025


![3D View](Generated/Archimedes_ARM6_3D_View.PNG)

An experimental platform adapting an ARM2 PLCC pinout to support an ARM610 or ARM710.

Built and tested in A3000, A310 and A540 (with my 'ARM2' adapter).  An unmodified RISC OS 3.1 fails POST as expected (PPL error, because Arm610/710 has no TRANS pin so no external PPL possible) but if allowed to continue RISC OS does run and the desktop can be used.

Until the cache can be enabled (software in development!), the fast clock is not used, so the part is running at MEMC speed (8MHz nominally).  But it's still slower than ARM2 (~65% speed) and I believe that may be because of the necessary 'SEQ' bodging for VIDC-area access.  TBC.


## Licence

No warranty is provided, and this work is used at your own risk.  

Licenced as CC BY-SA 4.0

Copyright 2025 Ian Jeffray

