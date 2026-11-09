# Troubleshooting log

Every problem I hit in the lab, newest first.

| Date | Lab | Problem | Cause | Fix |
| --- | --- | --- | --- | --- |
| 2026-11-05 | 00 | The Ubuntu installer failed at "installing kernel." | The 20 GB virtual disk was too small for Ubuntu Server 26.04.1. | Increased the virtual disk to 30 GB and reinstalled. |
| 2026-11-05 | 00 | PowerShell said `shh` is not recognized. | A typo in the command name. | Used `ssh`. |
| 2026-11-04 | 00 | Windows rejected the subnet mask as not contiguous. | A leftover digit from the auto-filled mask. | Retyped all four boxes as 255.255.255.0. |
