# Get-UNCPath-from-Hostname-and-local-path
Powershell Function to get UNCPath from Hostname and local path

# How to use

- Load the function (use dot net sourcing or copy the function in your script) and call like in the below example

```powershell
Get-UNCPath -Hostname Server01 -LocalPath "C:\temp\My test folder"
```

And a return from the above call will be :

```output
\\Server01\C$\temp\My test Folder
```

You can put the return in a variable for future use as well

```powershell
$UNCPath = Get-UNCPath -Hostname Server01 -LocalPath "C:\temp\My test folder"
```

and then the result aka the UNC path string will be stored in the above $UNCPath variable:

```output
[PS] C:\SCripts>$UNCPath
\\Server01\C$\temp\My test Folder
```
