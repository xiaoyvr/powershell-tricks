# Run Remote Script from Host

When you have windows VM share the user folder with Host OS. The $Profile will be someting like this.
```
\\psf\Home\Documents\WindowsPowerShell\Microsoft.PowerShell_profile.ps1
```
Everytime when you open powshell, you will get something like this.
```
Security Warning
Run only scripts that you trust. While scripts from the Internet can be useful, this script can potentially harm your computer. Do you want to run \\psf\Home\Documents\WindowsPowerShell\Microsoft.PowerShell_profile.ps1?
[D] Do not run  [R] Run once  [S] Suspend  [?] Help (default is "D"):
```

Run `Set-ExecutionPolicy Bypass`
```
Execution Policy Change
The execution policy helps protect you from scripts that you do not trust. Changing the execution policy might expose
you to the security risks described in the about_Execution_Policies help topic. Do you want to change the execution
policy?
[Y] Yes  [N] No  [S] Suspend  [?] Help (default is "Y"):
```
and answer "Y".
Then the security warning will be ignored.
