# bitlocker documentation

## ⭐introduction 

1. BitLocker is the Windows encryption technology.
2. BitLocker is free and built-in encryption solution designed for Windows operating systems.
3. It is available on Windows 10 or 11 Pro, Enterprise, Education.
4. It protects the drives of the computer from unauthorized access.
5. BitLocker helps protect the entire operating system drive against offline attacks.

## ⭐diving in practical scenarios

1. Normally when you access your data it's through Windows and has the usual protections associated with signing into Windows. 
2. If somebody wants to bypass those Windows protections, however, they could open the computer case and remove the physical hard drive. 
3. Then by adding your hard drive as a second drive on a machine they control, they may be able to access your data without needing your credentials.
4. If your drive is encrypted, however, when they try to use that method to access the drive, they'll have to provide the decryption key (which they shouldn't have) in order to access anything on the drive. 
5. Without the decryption key the data on the drive will just look like gibberish to them. 

## ⭐know your bitlocker key

1. bitlocker key is a unique 48 digit numeric password
2. bitlocker key remains saved in the personal microsoft account which is connected to your system
3. so by logging into your personal microsoft account you can get access to your bitlocker key
- go to devices 
- then go to recovery key 
4. if windows found that there is some unauthorised access to the windows then it might ask you your bitlocker recovery key to cross verify the authorisation.
5. also microsoft doesnot have any of your bitlocker recovery key nor it will regenerate your recovery key and hence you should have a backed up bitlocker recovery key.

## ⭐parting notes

1. In most situations your key is backed up when BitLocker is first turned on.
2. but we should have our bitlocker key as well
3. either save it in your personal microsoft account or file or write it with pen in notebook or save it in usb flash drive.
 
