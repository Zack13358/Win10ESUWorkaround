# Win10ESUWorkarounds
Satya Nadela's Extended Security Asscrack

Run the ESUcheck.bat file  
"cmd /c ClipESUConsumer.exe -evaluateEligibility" refreshes ESU eligibility  
"reg.exe query "HKCU\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Windows\ConsumerESU"" checks eligibility  

– “ESUEligibility” value mapping:

0: Unknown / Feature is not enabled  
1: Ineligible  
2: Eligible  
3: DeviceEnrolled  
5: MSAEnrolled  
8: LoginWithPrimaryAccountToEnroll  

– “ESUEligibilityResult” value mapping:

1: Success  
3: Non-Consumer edition  
4: Commercial device  
5: Non-Admin account  
6: Child account  
7: User Region is Embargoed  
8: Azure device  
11: Unknown / Feature is not enabled  
