# PVE-kernel-for-mlx3


A patched kernel for PVE7 that allows MLX3 (e.g., MLX354, HP544+) to pass through VF to Windows 10 guests.


It is recommended to use Windows 10 LTSC version. I am using Windows10 LTSC 2019, which has been stable for more than 6 months, and I have not tested it on any other version.

The ZFS module in the PVE has its own modified parts. I have not used ZFS in this kernel, so I am not certain about its stability. The sr-iov or gvt-g features of the i915 module may have issues, but since I don't need this function, I haven't made any fixes. Currently, I have patched the Linux kernel version 6, but I haven't used it extensively, so I am unsure about its stability, which is why I haven't uploaded it.



The patch originates from https://forums.servethehome.com/index.php?threads/help-with-connectx-3-sr-iov-with-linux-host-and-windows-guest-via-kvm.28956/, allowing you to create your custom kernel.


