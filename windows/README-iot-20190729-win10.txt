Belcarra USBLAN for Microsoft Windows OEM Distribution Kit 
Belcarra Technologies 2005

This package contains the Belcarra USBLAN driver for Windows 10.

The driver package is configured to your requirements using the options from:

        iot-20190729.xls

The following zip file contains the re-distributable End-User Kit for Windows 10:

        iot-20190729-win10.zip

These drivers are signed by Microsoft.

Windows 10 Kits can be made available from Windows Update. Contact Belcarra for
details.

When the USB Device is plugged in Windows will attempt to find the drivers on
Windows Update. When found the drivers are downloaded and installed for the
device.


The contents of this archive may be distributed on a CD or similar media 



End-User Redistribution Kit Contents
************************************

Archive:  iot-20190729-win10.zip
  Length      Date    Time    Name
---------  ---------- -----   ----
      925  10-28-2019 14:22   README-INSTALL.txt
     4888  10-28-2019 14:22   License.txt
     4493  10-28-2019 14:22   setup.bat
  1055168  10-28-2019 14:22   dpinst-x64.exe
   929728  10-28-2019 14:22   dpinst-x86.exe
---------                     -------
  1995202                     5 files



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


