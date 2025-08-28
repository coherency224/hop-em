.. Troubleshooting:

Troubleshooting - Optics degraded on Talos F200c
==========================

:Author: homewood cryoem
:Date-created: 2025-7-18
:Last-updated: 2025-8-28

Concurrent Optics degraded error (no beam), and Ceta cooling error.

Option #1

1. Close column valves, retract detector
2. In Microscope software launcher, right click the microscope icon, select Stop All. Wait until the status becomes 'stopped'
3. In Microscope software launcher, right click the microscope icon, select Start server and applications. Wait until the status becomes 'started'
4. Microscope software launcher -> Tools -> Camera and detector -> Ceta service Tool, Or open Ceta service tool from the taskbar shortcut. Select CSU tab in the Ceta service tool -> Show details -> Clear history. If successful, Ceta cooling will become Active. Wait for the temperature to reach -18C, before inserting the camera.
5. Microscope software launcher -> Tools -> Optics -> Optics Boards Diagnostics and Control, check if all green. If it is recovered, then Software stat should be Operational. If not, try pressing Recover


Option #2
1. shutting down the TEM server
2. powering cycling the optics system
3. restarting the TEM server


Learning materials
==========================

https://github.com/coherency224/hop-em/blob/main/docs/_downloads/Sec_IIA.pdf

https://github.com/coherency224/hop-em/blob/main/docs/_downloads/tem_primer2011.pdf

:download:`Negative_staining<../_downloads/Sec_IIA.pdf>`.

:download:`TEM Primer<../_downloads/tem_primer2011.pdf>`.
