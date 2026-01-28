.. Troubleshooting:

Troubleshooting - Optics degraded on Talos F200c
==========================

:Author: homewood cryoem
:Date-created: 2025-7-18
:Last-updated: 2026-1-28

Concurrent Optics degraded error (no beam), and Ceta cooling error.

Option #1

1. Close column valves, retract detector
2. Microscope software launcher -> Tools -> Camera and detector -> Ceta service Tool, Or open Ceta service tool from the taskbar shortcut. Select CSU tab in the Ceta service tool -> Show details -> Clear history. If successful, Ceta cooling will become Active. Wait for the temperature to reach -18C, before inserting the camera.
3. Microscope software launcher -> Tools -> Optics -> Optics Boards Diagnostics and Control, check if all green. If not, presse 'Recover' near the bottom of the panel. If successful, all status should turn green. Check if the beam is visible on the fluscreen.

Option #2

1. Close column valves, retract detector
2. In Microscope software launcher, right click the microscope icon, select Stop All. Wait until the status becomes 'stopped'
3. In Microscope software launcher, right click the microscope icon, select Start server and applications. Wait until the status becomes 'started'
4. Microscope software launcher -> Tools -> Camera and detector -> Ceta service Tool, Or open Ceta service tool from the taskbar shortcut. Select CSU tab in the Ceta service tool -> Show details -> Clear history. If successful, Ceta cooling will become Active. Wait for the temperature to reach -18C, before inserting the camera.
5. Microscope software launcher -> Tools -> Optics -> Optics Boards Diagnostics and Control, check if all green. If it is recovered, then Software stat should be Operational. If not, try pressing Recover.


Option #3

1. shutting down the TEM server
2. powering cycling the optics system
3. restarting the TEM server

Troubleshooting - Vacuum crash
==========================

Vacuum crash can occur during holder exchange. It shuts down TMPp and IGPco. Ceta warms up due to loss of projection vacuum.

The system will attempt recovery automatically and Vacuum overview will show the progress.

1. Retract Ceta if it is inserted. 
2. Open the flapout of Vacuum control panel, go to Control tab, if 'Recover' button is clickable, press it. Wait and check the progress status in Vacuum overview. The system may activate 'To All Vacuum' (the button turns yellow) automatically after TMPp reaches full speed. If not, press 'To All Vacuum' (below 'Recover') when it is clickable. This should turn on IGPco. Wait for all items in Vacuum control panel to turn green. 
3. Check sensor temperature in Ceta service tool. The target temperature is -18C. Wait for the temperature to go down. It may fluctuate. You may proceed to insert Ceta when the temperature is below -17C. This may take an hour depending on the temperature that Ceta sensor rises to before cooling down again.
4. When column pressure recovers to below 20 log, you may open column valves and check the beam. 



Learning materials
==========================

https://www.youtube.com/@StructureClub

https://emx.stanford.edu/previous-speakers

https://github.com/coherency224/hop-em/blob/main/docs/_downloads/Sec_IIA.pdf

https://github.com/coherency224/hop-em/blob/main/docs/_downloads/tem_primer2011.pdf

https://documents.thermofisher.com/TFS-Assets/MSD/brochures/accelerating-drug-discovery-with-rational-design-brochure.pdf

Streamlined Workflows for Advanced Cryo-EM and Tomography
https://event.on24.com/wcc/r/5114520/697ADCF2355CC307459B2A8BF2DB5FA8

:download:`Negative_staining<../_downloads/Sec_IIA.pdf>`.

:download:`TEM Primer<../_downloads/tem_primer2011.pdf>`.


