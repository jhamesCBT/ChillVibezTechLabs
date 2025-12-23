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

