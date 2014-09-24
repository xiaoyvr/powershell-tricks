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

Use `Set-ExecutionPolicy Bypass` to ignore it.
