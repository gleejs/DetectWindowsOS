# DetectWindowsOS
Powershell to Detect 32 bit or 64 OS
https://social.technet.microsoft.com/Forums/office/en-US/5dfeb3ab-6265-40cd-a4ac-05428b9db5c3/determine-32-or-64bit-os?forum=winserverpowershell



$os = get-wmiobject -Class Win32_Processor
$os.addresswidth 

Will display 64


http://techibee.com/powershell/get-operating-system-architecture32-bit-or-64-bit-using-powershell/689

$os = get-wmiobject -Class Win32_OperatingSystem
$os.osarchitecture

Will display 64-Bit


https://blogs.msdn.microsoft.com/koteshb/2010/02/12/powershell-how-to-find-details-of-operating-system/


PS C:\> (Get-WmiObject Win32_OperatingSystem).OSArchitecture
