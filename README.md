

# Get Started
Order Lab here:
[https://Chillvibeztech.com](https://chillvibeztech.com/)


1. Sign up for Windows Trial and Download the ISO here:
([WindowsServerTrial](https://info.microsoft.com/ww-landing-evaluate-windows-server-2025.html?lcid=en-us&culture=en-us&country=us))


# Setup the Lab Environment
Create Virtual Machines
https://youtube.com/shorts/-ksF-eB7okk

For each lab Virtual Machine follow the Windows installation guide here:
https://youtube.com/shorts/mRFlOS7TIfg

# Build the Lab
Follow the steps in the content video here:
https://youtu.be/dukyOlMFK0E


Email if help is needed
jhames@chillvibeztech.com


///
HYPER V COMMAND

	Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Hyper-V -All

RESTART COMMAND

	SHUTDOWN /R /T 00

POLICY COMMAND

	Set-ExecutionPolicy RemoteSigned -Scope CurrentUser

LAB COMMAND
	
	$name = New-Item -Path Env:\LAB_NAME -Value 'Network_Lab' | Select-Object Value -ExpandProperty Value

EXTRACT COMMAND 

	Expand-Archive -Path $Env:USERPROFILE/Downloads/$name.zip -DestinationPath $Env:USERPROFILE/Downloads/$name

SETUP COMMAND

	powershell $Env:USERPROFILE\Downloads\$name\$name"_Setup.ps1"

TEARDOWN COMMAND

	powershell $Env:USERPROFILE\Downloads\$name\$name"_Teardown.ps1"

