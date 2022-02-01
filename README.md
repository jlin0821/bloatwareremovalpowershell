Get-AppxPackage -allusers Microsoft.549981C3F5F10 | Remove-AppxPackage

https://www.groovypost.com/howto/copy-paste-kindle-fire/

# bloatwareremovalpowershell

Windows PowerShell
Copyright (C) Microsoft Corporation. All rights reserved.

PS C:\WINDOWS\system32> 3D Builder: Get-AppxPackage *3dbuilder* | Remove-AppxPackage
>>
>> Alarms and Clock: Get-AppxPackage *windowsalarms* | Remove-AppxPackage
>>
>> Calculator: Get-AppxPackage *windowscalculator* | Remove-AppxPackage
>>
>> Calendar and Mail: Get-AppxPackage *windowscommunicationsapps* | Remove-AppxPackage
>>
>> Camera: Get-AppxPackage *windowscamera* | Remove-AppxPackage
>>
>> Get Office: Get-AppxPackage *officehub* | Remove-AppxPackage
>>
>> Get Skype: Get-AppxPackage *skypeapp* | Remove-AppxPackage
>>
>> Get Started: Get-AppxPackage *getstarted* | Remove-AppxPackage
>>
>> Groove Music: Get-AppxPackage *zunemusic* | Remove-AppxPackage
>>
>> Maps: Get-AppxPackage *windowsmaps* | Remove-AppxPackage
>>
>> Microsoft Solitaire Collection: Get-AppxPackage *solitairecollection* | Remove-AppxPackage
>>
>> Money: Get-AppxPackage *bingfinance* | Remove-AppxPackage
>>
>> Movies & TV: Get-AppxPackage *zunevideo* | Remove-AppxPackage
>>
>> News: Get-AppxPackage *bingnews* | Remove-AppxPackage
>>
>> OneNote: Get-AppxPackage *onenote* | Remove-AppxPackage
>>
>> People: Get-AppxPackage *people* | Remove-AppxPackage
>>
>> Phone Companion: Get-AppxPackage *windowsphone* | Remove-AppxPackage
>>
>> Photos: Get-AppxPackage *photos* | Remove-AppxPackage
>>
>> Store: Get-AppxPackage *windowsstore* | Remove-AppxPackage
>>
>> Sports: Get-AppxPackage *bingsports* | Remove-AppxPackage
>>
>> Voice Recorder: Get-AppxPackage *soundrecorder* | Remove-AppxPackage
>>
>> Weather: Get-AppxPackage *bingweather* | Remove-AppxPackage
>>
>> Xbox: Get-AppxPackage *xboxapp* | Remove-AppxPackage
>>
>>
At line:1 char:4
+ 3D Builder: Get-AppxPackage *3dbuilder* | Remove-AppxPackage
+    ~~~~~~~~
Unexpected token 'Builder:' in expression or statement.
At line:25 char:8
+ Movies & TV: Get-AppxPackage *zunevideo* | Remove-AppxPackage
+        ~
The ampersand (&) character is not allowed. The & operator is reserved for future use; wrap an ampersand in double
quotation marks ("&") to pass it as part of a string.
    + CategoryInfo          : ParserError: (:) [], ParentContainsErrorRecordException
    + FullyQualifiedErrorId : UnexpectedToken

PS C:\WINDOWS\system32> Xbox: Get-AppxPackage *xboxapp* | Remove-AppxPackage
>>
>>
Xbox: : The term 'Xbox:' is not recognized as the name of a cmdlet, function, script file, or operable program. Check
the spelling of the name, or if a path was included, verify that the path is correct and try again.
At line:1 char:1
+ Xbox: Get-AppxPackage *xboxapp* | Remove-AppxPackage
+ ~~~~~
    + CategoryInfo          : ObjectNotFound: (Xbox::String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException

PS C:\WINDOWS\system32> Xbox: Get-AppxPackage *xboxapp* | Remove-AppxPackage
Xbox: : The term 'Xbox:' is not recognized as the name of a cmdlet, function, script file, or operable program. Check
the spelling of the name, or if a path was included, verify that the path is correct and try again.
At line:1 char:1
+ Xbox: Get-AppxPackage *xboxapp* | Remove-AppxPackage
+ ~~~~~
    + CategoryInfo          : ObjectNotFound: (Xbox::String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException

PS C:\WINDOWS\system32> Get-AppxPackage *xboxapp* | Remove-AppxPackage
PS C:\WINDOWS\system32> Get-AppxPackage *bingweather* | Remove-AppxPackage
PS C:\WINDOWS\system32> Get-AppxPackage *zunevideo* | Remove-AppxPackage
PS C:\WINDOWS\system32> Get-AppxPackage *windowscamera* | Remove-AppxPackage
PS C:\WINDOWS\system32> Get-AppxPackage *officehub* | Remove-AppxPackage
PS C:\WINDOWS\system32> Get-AppxPackage *getstarted* | Remove-AppxPackage
PS C:\WINDOWS\system32> Get-AppxPackage *zunemusic* | Remove-AppxPackage
PS C:\WINDOWS\system32> Get-AppxPackage *solitairecollection* | Remove-AppxPackage
PS C:\WINDOWS\system32> Get-AppxPackage *bingfinance* | Remove-AppxPackage
PS C:\WINDOWS\system32> Get-AppxPackage *zunevideo* | Remove-AppxPackage
PS C:\WINDOWS\system32> Get-AppxPackage *people* | Remove-AppxPackage
Remove-AppxPackage : Deployment failed with HRESULT: 0x80073CFA, Removal failed. Please contact your software vendor.
(Exception from HRESULT: 0x80073CFA)
error 0x80070032: AppX Deployment Remove operation on package
Microsoft.Windows.PeopleExperienceHost_10.0.17134.1_neutral_neutral_cw5n1h2txyewy from:
C:\Windows\SystemApps\Microsoft.Windows.PeopleExperienceHost_cw5n1h2txyewy failed. This app is part of Windows and
cannot be uninstalled on a per-user basis. An administrator can attempt to remove the app from the computer using Turn
Windows Features on or off. However, it may not be possible to uninstall the app.
NOTE: For additional information, look for [ActivityId] 6a7b0baf-7eb5-0002-1380-866ab57ed501 in the Event Log or use
the command line Get-AppxLog -ActivityID 6a7b0baf-7eb5-0002-1380-866ab57ed501
At line:1 char:28
+ Get-AppxPackage *people* | Remove-AppxPackage
+                            ~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : WriteError: (Microsoft.Windo...l_cw5n1h2txyewy:String) [Remove-AppxPackage], IOException
    + FullyQualifiedErrorId : DeploymentError,Microsoft.Windows.Appx.PackageManager.Commands.RemoveAppxPackageCommand

PS C:\WINDOWS\system32> Get-AppxPackage *photos* | Remove-AppxPackage
PS C:\WINDOWS\system32> Get-AppxPackage *bingsports* | Remove-AppxPackage
PS C:\WINDOWS\system32> DISM /Online /Get-ProvisionedAppxPackages | select-string Packagename
>>

PackageName : Microsoft.BingWeather_4.32.12463.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.DesktopAppInstaller_2019.515.2246.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.GetHelp_10.1706.22112.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.Getstarted_6.15.12641.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.Messaging_2019.125.32.1000_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.Microsoft3DViewer_7.1908.9012.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.MicrosoftOfficeHub_18.1903.1152.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.MicrosoftSolitaireCollection_4.4.10022.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.MicrosoftStickyNotes_3.7.71.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.MSPaint_2019.718.2251.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.Office.OneNote_16001.12130.20090.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.OneConnect_5.1906.1791.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.People_2019.305.632.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.Print3D_3.3.791.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.SkypeApp_14.53.85.0_neutral_~_kzf8qxf38zg5c
PackageName : Microsoft.StorePurchaseApp_11910.1001.413.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.Wallet_2.2.18065.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.WebMediaExtensions_1.0.13321.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.Windows.Photos_2019.19071.17920.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.WindowsAlarms_2019.716.2337.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.WindowsCalculator_2020.1908.0.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.WindowsCamera_2019.821.30.0_neutral_~_8wekyb3d8bbwe
PackageName : microsoft.windowscommunicationsapps_16005.12026.20218.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.WindowsFeedbackHub_2019.821.2153.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.WindowsMaps_2019.716.2316.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.WindowsSoundRecorder_2019.905.2222.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.WindowsStore_11910.1001.513.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.Xbox.TCUI_1.24.10001.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.XboxApp_48.58.11001.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.XboxGameOverlay_1.46.11001.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.XboxGamingOverlay_1.16.1012.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.XboxIdentityProvider_12.54.26001.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.XboxSpeechToTextOverlay_1.21.13002.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.ZuneMusic_2019.19072.18011.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.ZuneVideo_2019.19072.18011.0_neutral_~_8wekyb3d8bbwe


PS C:\WINDOWS\system32> DISM /Online /Remove-ProvisionedAppxPackage /PackageName:Microsoft.ZuneVideo_2019.19072.18011.0_neutral_~_8wekyb3d8bbwe

Deployment Image Servicing and Management tool
Version: 10.0.17134.1

Image Version: 10.0.17134.1069

The operation completed successfully.
PS C:\WINDOWS\system32> DISM /Online /Remove-ProvisionedAppxPackage /PackageName:Microsoft.BingWeather_4.32.12463.0_neutral_~_8wekyb3d8bbwe

Deployment Image Servicing and Management tool
Version: 10.0.17134.1

Image Version: 10.0.17134.1069

The operation completed successfully.
PS C:\WINDOWS\system32> DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.GetHelp_10.1706.22112.0_neutral_~_8wekyb3d8bbwe
>>  DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.Getstarted_6.15.12641.0_neutral_~_8wekyb3d8bbwe
>>  DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.Messaging_2019.125.32.1000_neutral_~_8wekyb3d8bbwe
>>  DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.MicrosoftOfficeHub_18.1903.1152.0_neutral_~_8wekyb3d8bbwe
>>  DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.MicrosoftSolitaireCollection_4.4.10022.0_neutral_~_8wekyb3d8bbwe
>>  DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.MicrosoftStickyNotes_3.7.71.0_neutral_~_8wekyb3d8bbwe
>>  DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.OneConnect_5.1906.1791.0_neutral_~_8wekyb3d8bbwe
>>  DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.People_2019.305.632.0_neutral_~_8wekyb3d8bbwe
>>  DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.Wallet_2.2.18065.0_neutral_~_8wekyb3d8bbwe
>>  DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.WebMediaExtensions_1.0.13321.0_neutral_~_8wekyb3d8bbwe
>>  DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.Windows.Photos_2019.19071.17920.0_neutral_~_8wekyb3d8bbwe
>>  DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.WindowsAlarms_2019.716.2337.0_neutral_~_8wekyb3d8bbwe
>>  DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.WindowsCamera_2019.821.30.0_neutral_~_8wekyb3d8bbwe
>>  DISM /Online /Remove-ProvisionedAppxPackage /PackageName : microsoft.windowscommunicationsapps_16005.12026.20218.0_neutral_~_8wekyb3d8bbwe
>>  DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.WindowsFeedbackHub_2019.821.2153.0_neutral_~_8wekyb3d8bbwe
>>  DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.WindowsMaps_2019.716.2316.0_neutral_~_8wekyb3d8bbwe
>>  DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.Xbox.TCUI_1.24.10001.0_neutral_~_8wekyb3d8bbwe>>  DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.XboxApp_48.58.11001.0_neutral_~_8wekyb3d8bbwe
>>  DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.XboxGameOverlay_1.46.11001.0_neutral_~_8wekyb3d8bbwe
>>  DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.XboxGamingOverlay_1.16.1012.0_neutral_~_8wekyb3d8bbwe
>>  DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.XboxIdentityProvider_12.54.26001.0_neutral_~_8wekyb3d8bbwe
>>  DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.XboxSpeechToTextOverlay_1.21.13002.0_neutral_~_8wekyb3d8bbwe
>>  DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.ZuneMusic_2019.19072.18011.0_neutral_~_8wekyb3d8bbwe


Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log
PS C:\WINDOWS\system32> DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.GetHelp_10.1706.22112.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.Getstarted_6.15.12641.0_neutral_~_8wekyb3d8bbwe>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.Messaging_2019.125.32.1000_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.MicrosoftOfficeHub_18.1903.1152.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.MicrosoftSolitaireCollection_4.4.10022.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.MicrosoftStickyNotes_3.7.71.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.OneConnect_5.1906.1791.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.People_2019.305.632.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.Wallet_2.2.18065.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.WebMediaExtensions_1.0.13321.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.Windows.Photos_2019.19071.17920.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.WindowsAlarms_2019.716.2337.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.WindowsCamera_2019.821.30.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName : microsoft.windowscommunicationsapps_16005.12026.20218.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.WindowsFeedbackHub_2019.821.2153.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.WindowsMaps_2019.716.2316.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.Xbox.TCUI_1.24.10001.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.XboxApp_48.58.11001.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.XboxGameOverlay_1.46.11001.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.XboxGamingOverlay_1.16.1012.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.XboxIdentityProvider_12.54.26001.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.XboxSpeechToTextOverlay_1.21.13002.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName : Microsoft.ZuneMusic_2019.19072.18011.0_neutral_~_8wekyb3d8bbwe


Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

DISM doesn't recognize the command-line option ":".
For more information, refer to the help by running DISM.exe /?.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log
PS C:\WINDOWS\system32> DISM /Online /Remove-ProvisionedAppxPackage /PackageName: Microsoft.GetHelp_10.1706.22112.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName: Microsoft.Getstarted_6.15.12641.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName: Microsoft.Messaging_2019.125.32.1000_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName: Microsoft.MicrosoftOfficeHub_18.1903.1152.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName: Microsoft.MicrosoftSolitaireCollection_4.4.10022.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName: Microsoft.MicrosoftStickyNotes_3.7.71.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName: Microsoft.OneConnect_5.1906.1791.0_neutral_~_8wekyb3d8bbwe>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName: Microsoft.People_2019.305.632.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName: Microsoft.Wallet_2.2.18065.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName: Microsoft.WebMediaExtensions_1.0.13321.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName: Microsoft.Windows.Photos_2019.19071.17920.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName: Microsoft.WindowsAlarms_2019.716.2337.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName: Microsoft.WindowsCamera_2019.821.30.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName: microsoft.windowscommunicationsapps_16005.12026.20218.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName: Microsoft.WindowsFeedbackHub_2019.821.2153.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName: Microsoft.WindowsMaps_2019.716.2316.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName: Microsoft.Xbox.TCUI_1.24.10001.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName: Microsoft.XboxApp_48.58.11001.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName: Microsoft.XboxGameOverlay_1.46.11001.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName: Microsoft.XboxGamingOverlay_1.16.1012.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName: Microsoft.XboxIdentityProvider_12.54.26001.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName: Microsoft.XboxSpeechToTextOverlay_1.21.13002.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName: Microsoft.ZuneMusic_2019.19072.18011.0_neutral_~_8wekyb3d8bbwe


Error: 87

The /PackageName: option is missing a required argument.
For more information, refer to the help for the /PackageName: option.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

The /PackageName: option is missing a required argument.
For more information, refer to the help for the /PackageName: option.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

The /PackageName: option is missing a required argument.
For more information, refer to the help for the /PackageName: option.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

The /PackageName: option is missing a required argument.
For more information, refer to the help for the /PackageName: option.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

The /PackageName: option is missing a required argument.
For more information, refer to the help for the /PackageName: option.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

The /PackageName: option is missing a required argument.
For more information, refer to the help for the /PackageName: option.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

The /PackageName: option is missing a required argument.
For more information, refer to the help for the /PackageName: option.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

The /PackageName: option is missing a required argument.
For more information, refer to the help for the /PackageName: option.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

The /PackageName: option is missing a required argument.
For more information, refer to the help for the /PackageName: option.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

The /PackageName: option is missing a required argument.
For more information, refer to the help for the /PackageName: option.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

The /PackageName: option is missing a required argument.
For more information, refer to the help for the /PackageName: option.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

The /PackageName: option is missing a required argument.
For more information, refer to the help for the /PackageName: option.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

The /PackageName: option is missing a required argument.
For more information, refer to the help for the /PackageName: option.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

The /PackageName: option is missing a required argument.
For more information, refer to the help for the /PackageName: option.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

The /PackageName: option is missing a required argument.
For more information, refer to the help for the /PackageName: option.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

The /PackageName: option is missing a required argument.
For more information, refer to the help for the /PackageName: option.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

The /PackageName: option is missing a required argument.
For more information, refer to the help for the /PackageName: option.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

The /PackageName: option is missing a required argument.
For more information, refer to the help for the /PackageName: option.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

The /PackageName: option is missing a required argument.
For more information, refer to the help for the /PackageName: option.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

The /PackageName: option is missing a required argument.
For more information, refer to the help for the /PackageName: option.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

The /PackageName: option is missing a required argument.
For more information, refer to the help for the /PackageName: option.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

The /PackageName: option is missing a required argument.
For more information, refer to the help for the /PackageName: option.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Error: 87

The /PackageName: option is missing a required argument.
For more information, refer to the help for the /PackageName: option.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log
PS C:\WINDOWS\system32> DISM /Online /Remove-ProvisionedAppxPackage /PackageName: Microsoft.ZuneMusic_2019.19072.18011.0_neutral_~_8wekyb3d8bbwe

Error: 87

The /PackageName: option is missing a required argument.
For more information, refer to the help for the /PackageName: option.

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log
PS C:\WINDOWS\system32> DISM /Online /Remove-ProvisionedAppxPackage /PackageName:Microsoft.XboxGamingOverlay_1.16.1012.0_neutral_~_8wekyb3d8bbwe

Deployment Image Servicing and Management tool
Version: 10.0.17134.1

Image Version: 10.0.17134.1069

The operation completed successfully.
PS C:\WINDOWS\system32> DISM /Online /Remove-ProvisionedAppxPackage /PackageName:Microsoft.GetHelp_10.1706.22112.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName:Microsoft.Getstarted_6.15.12641.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName:Microsoft.Messaging_2019.125.32.1000_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName:Microsoft.MicrosoftOfficeHub_18.1903.1152.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName:Microsoft.MicrosoftSolitaireCollection_4.4.10022.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName:Microsoft.MicrosoftStickyNotes_3.7.71.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName:Microsoft.OneConnect_5.1906.1791.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName:Microsoft.People_2019.305.632.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName:Microsoft.Wallet_2.2.18065.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName:Microsoft.WebMediaExtensions_1.0.13321.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName:Microsoft.Windows.Photos_2019.19071.17920.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName:Microsoft.WindowsAlarms_2019.716.2337.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName:Microsoft.WindowsCamera_2019.821.30.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName:microsoft.windowscommunicationsapps_16005.12026.20218.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName:Microsoft.WindowsFeedbackHub_2019.821.2153.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName:Microsoft.WindowsMaps_2019.716.2316.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName:Microsoft.Xbox.TCUI_1.24.10001.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName:Microsoft.XboxApp_48.58.11001.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName:Microsoft.XboxGameOverlay_1.46.11001.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName:Microsoft.XboxGamingOverlay_1.16.1012.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName:Microsoft.XboxIdentityProvider_12.54.26001.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName:Microsoft.XboxSpeechToTextOverlay_1.21.13002.0_neutral_~_8wekyb3d8bbwe
>> DISM /Online /Remove-ProvisionedAppxPackage /PackageName:Microsoft.ZuneMusic_2019.19072.18011.0_neutral_~_8wekyb3d8bbwe

Deployment Image Servicing and Management tool
Version: 10.0.17134.1

Image Version: 10.0.17134.1069

The operation completed successfully.

Deployment Image Servicing and Management tool
Version: 10.0.17134.1

Image Version: 10.0.17134.1069

The operation completed successfully.

Deployment Image Servicing and Management tool
Version: 10.0.17134.1

Image Version: 10.0.17134.1069

The operation completed successfully.

Deployment Image Servicing and Management tool
Version: 10.0.17134.1

Image Version: 10.0.17134.1069

The operation completed successfully.

Deployment Image Servicing and Management tool
Version: 10.0.17134.1

Image Version: 10.0.17134.1069

The operation completed successfully.

Deployment Image Servicing and Management tool
Version: 10.0.17134.1

Image Version: 10.0.17134.1069

The operation completed successfully.

Deployment Image Servicing and Management tool
Version: 10.0.17134.1

Image Version: 10.0.17134.1069

The operation completed successfully.

Deployment Image Servicing and Management tool
Version: 10.0.17134.1

Image Version: 10.0.17134.1069

The operation completed successfully.

Deployment Image Servicing and Management tool
Version: 10.0.17134.1

Image Version: 10.0.17134.1069

The operation completed successfully.

Deployment Image Servicing and Management tool
Version: 10.0.17134.1

Image Version: 10.0.17134.1069

The operation completed successfully.

Deployment Image Servicing and Management tool
Version: 10.0.17134.1

Image Version: 10.0.17134.1069

The operation completed successfully.

Deployment Image Servicing and Management tool
Version: 10.0.17134.1

Image Version: 10.0.17134.1069

The operation completed successfully.

Deployment Image Servicing and Management tool
Version: 10.0.17134.1

Image Version: 10.0.17134.1069

The operation completed successfully.

Deployment Image Servicing and Management tool
Version: 10.0.17134.1

Image Version: 10.0.17134.1069

The operation completed successfully.

Deployment Image Servicing and Management tool
Version: 10.0.17134.1

Image Version: 10.0.17134.1069

The operation completed successfully.

Deployment Image Servicing and Management tool
Version: 10.0.17134.1

Image Version: 10.0.17134.1069

The operation completed successfully.

Deployment Image Servicing and Management tool
Version: 10.0.17134.1

Image Version: 10.0.17134.1069

The operation completed successfully.

Deployment Image Servicing and Management tool
Version: 10.0.17134.1

Image Version: 10.0.17134.1069

The operation completed successfully.

Deployment Image Servicing and Management tool
Version: 10.0.17134.1

Image Version: 10.0.17134.1069

The operation completed successfully.

Deployment Image Servicing and Management tool
Version: 10.0.17134.1

Image Version: 10.0.17134.1069


Error: 2

Unspecified error

The DISM log file can be found at C:\WINDOWS\Logs\DISM\dism.log

Deployment Image Servicing and Management tool
Version: 10.0.17134.1

Image Version: 10.0.17134.1069

The operation completed successfully.

Deployment Image Servicing and Management tool
Version: 10.0.17134.1

Image Version: 10.0.17134.1069

The operation completed successfully.

Deployment Image Servicing and Management tool
Version: 10.0.17134.1

Image Version: 10.0.17134.1069

The operation completed successfully.
PS C:\WINDOWS\system32> DISM /Online /Get-ProvisionedAppxPackages | select-string Packagename
>>

PackageName : Microsoft.DesktopAppInstaller_2019.515.2246.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.Microsoft3DViewer_7.1908.9012.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.MSPaint_2019.718.2251.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.Office.OneNote_16001.12130.20090.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.Print3D_3.3.791.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.SkypeApp_14.53.85.0_neutral_~_kzf8qxf38zg5c
PackageName : Microsoft.StorePurchaseApp_11910.1001.413.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.WindowsCalculator_2020.1908.0.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.WindowsSoundRecorder_2019.905.2222.0_neutral_~_8wekyb3d8bbwe
PackageName : Microsoft.WindowsStore_11910.1001.513.0_neutral_~_8wekyb3d8bbwe

credit: https://www.makeuseof.com/tag/easily-remove-bloatware-windows-10/
