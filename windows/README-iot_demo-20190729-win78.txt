Belcarra USBLAN for Microsoft Windows OEM Distribution Kit 
Belcarra Technologies 2005

This package contains the Belcarra USBLAN driver for Windows 7 and Windows 8.

The driver package is configured to your requirements using the options from the
following spreadsheet, which is also included in this kit:

        iot_demo-20190729.xls

The following zip file contains the re-distributable End-User Kit:

        iot_demo-20190729-win78.zip

These drivers are signed by Belcarra and will will install on Windows 7 and 
Windows 8 with an Unknown Publisher Warning.


End-User Redistribution Kit Contents
************************************

Archive:  iot_demo-20190729-win78.zip
  Length      Date    Time    Name
---------  ---------- -----   ----
    85611  10-28-2019 13:59   README-Windows7-SecurityUpdate-KB30339290.pdf
      925  10-28-2019 13:59   README-INSTALL.txt
      346  10-28-2019 13:59   README-WinXP-unsigned.txt
     4888  10-28-2019 13:59   License.txt
     4493  10-28-2019 13:59   setup.bat
  1055168  10-28-2019 13:59   dpinst-x64.exe
   929728  10-28-2019 13:59   dpinst-x86.exe
        0  10-28-2019 13:59   vista/amd64/
   757760  10-28-2019 13:59   vista/amd64/iotdemo.pdb
    73728  10-28-2019 13:59   vista/amd64/iotdemo.sys
        0  10-28-2019 13:59   vista/i386/
   765952  10-28-2019 13:59   vista/i386/iotdemo.pdb
    57856  10-28-2019 13:59   vista/i386/iotdemo.sys
     9598  10-28-2019 13:59   vista/iot_demo.inf
        0  10-28-2019 13:59   win7/amd64/
   798720  10-28-2019 13:59   win7/amd64/iotdemo.pdb
    85720  10-28-2019 13:59   win7/amd64/iotdemo.sys
        0  10-28-2019 13:59   win7/i386/
   798720  10-28-2019 13:59   win7/i386/iotdemo.pdb
    69336  10-28-2019 13:59   win7/i386/iotdemo.sys
    11254  10-28-2019 13:59   win7/iot_demo.cat
     8846  10-28-2019 13:59   win7/iot_demo.inf
        0  10-28-2019 13:59   win8/amd64/
   815104  10-28-2019 13:59   win8/amd64/iotdemo.pdb
    85720  10-28-2019 13:59   win8/amd64/iotdemo.sys
        0  10-28-2019 13:59   win8/i386/
   815104  10-28-2019 13:59   win8/i386/iotdemo.pdb
    69336  10-28-2019 13:59   win8/i386/iotdemo.sys
    11529  10-28-2019 13:59   win8/iot_demo.cat
     8846  10-28-2019 13:59   win8/iot_demo.inf
---------                     -------
  7324288                     30 files



Installation
************

There are several common scenarios for installation of these drivers.

When a USB Device is plugged in Windows will do the following:

    1. Look for a previously used driver
    2. Look for a pre-loaded but not in use driver
    3. Look for the driver in Windows Update
    4. Fail

If Windows fails to find a driver the user can interact with the Device Manager
to direct Windows to look for a driver in a specific place, typically by
browsing to a folder containing the drivers.

A. Pre-Install from Disk 
************************

The drivers can be pre-installed using the Microsoft DPInst utility. This is
done by using the setup.bat script in the archive. DPInst copies the drivers to
an archive location. Later Windows will be able to find the drivers when your
device is plugged in.

For more information see:

    http://www.microsoft.com/whdc/driver/install/difxtools.mspx

This can be done with both the cross-signed kit from Belcarra and the optional
Microsoft Signed kit

B. Directed Install from Disk
*****************************

Older versions of Windows (e.g. Windows XP) allow for the user to specify the
location of the drivers during the initial installation process (by browsing to
where the zip archive is unpacked).

 N.B New versions of Windows (e.g. Windows 7) do not allow this in the initial
 installation phase. 

If Windows does not find the driver (because neither of the first two
installation options was used) the driver can be installed by using the Windows
Device Manager.

Navigate to Control Panel / System / Hardware / Device manager and find the
"unknown device". Then "update drivers" can be used to find and install the
drivers from the CD or directory containing the driver installation files
(contents of the driver000 directory).

This method can also be used to update drivers, in that case using the uninstall
or update menu items.

This can be done with both the cross-signed kit from Belcarra and the optional
Microsoft Signed kit


More Information
****************

More information can be found on the websites:

    - http://www.belcarra.com/
    - http://usblan.belcarra.com/


--
Last updated May 2017


