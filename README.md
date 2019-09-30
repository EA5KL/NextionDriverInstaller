NextionDriver Installer and Checker
===================================

This is installer version 1.04 ( 16 aug 2019 )

This repository brings you 3 helper programs for the installation of
NextionDriver when you do not want to do it by hand:

 * a program to install NextionDriver
 * a program to convert an existing MMDVMHost configuration file for
   using NextionDriver (this is called by the installer program)
 * a program to check the installation

-----
__Please use this installer to update your system if your installation is
older than this date. Even if the NextionDriver was recently updated__

-----


### install.sh

This is the installer program for NextionDriver.

I (and others) have tested it on some hotspots, but there are always
much more situations and combinations than the ones we tested :-)
(special thanks to Rob PD0DIB for his feedback)

The installer runs the configuration convertor program for automatically
converting the MMDVM.ini file to incorporate NextionDriver.


### NextionDriver_ConvertConfig

You could just run it (NextionDriver_ConvertConfig) if you installed
NextionDriver by hand, but it also will be called when you run the
installer !

### check_installation.sh

When you have installed the NextionDriver, this programs tries to check
the  MMDVMHost and NextionDriver configuration.  
The program then gives a lot of information about the installation
of the NextionDriver and if it seems to be OK or not.




## Installing NextionDriver (on Pi-Star)

log in to your Pi-Star with SSH

* use PuTTY
* or go to your dashboard -> configuration -> expert -> SSH access
  (http://pi-star.local/admin/expert/ssh_access.php)

go to the /tmp directory
```
cd /tmp
```

get the software
```
git clone https://github.com/ElGamal/NextionDriverInstaller.git
```

go !
```
sudo NextionDriverInstaller/install.sh
```


## Checking the installing (on Pi-Star)

log in to your Pi-Star with SSH

* use PuTTY
* or go to your dashboard -> configuration -> expert -> SSH access (http://pi-star.local/admin/expert/ssh_access.php)

go to the /tmp directory
```
cd /tmp
```

get the software
```
git clone https://github.com/ElGamal/NextionDriverInstaller.git
```
>NOTE: if you get an error that the destionation path exists,
>you already downloaded the software. The just ho to the next step.

go !
```
sudo NextionDriverInstaller/check_installation.sh
```
