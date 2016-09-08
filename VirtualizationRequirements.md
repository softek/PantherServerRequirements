Virtual Environment Requirements:
* The virtualization software supports USB pass-through from the VM host to the VMs. This is required to support the use of a WIBU security dongle that Panther accesses regularly.
* Host
  * ESXi 4.1
* Resources are devoted to the Panther VM and NOT shared.

Virtual Machine #1 (Panther services):
* Hard drive
  * 128 GB Volume for OS, formatted to use the system default block size
  * 500 IOPS
  * Minimum 80MB/s Sustained Transfer Rate (STR)
* RAM
  * 8 GB
* CPU
  * Modern Nehalem, Core, 65nm Opteron or equivalent processors
  * 16 logical processors
* Network
  * 1 Gigabit connection & static IP

Virtual Machine #2 (Database services):
* Hard drive
  * 1 x 300 GB
* RAM
  * 16 GB
* CPU
  * 4 logical cores
* Network
  * 1 Gigabit connection
  * static IP

v7.0