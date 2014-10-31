# About Dot Sourcing

Use `.` (dot sourcing) to include file. It will only be included in current scope. This means you cannot write a function to include a file, and use it outside this function. Because it only visible within the function instead of the callilng context.

What you can do is to use another `.` to open the function also.

```ps
# Get-Foo.ps1
function Get-Foo{
  write-host "getting foo"
}

```

```ps
function IncludingFile{
  . "./Get-Foo.ps1"
}

```

```ps
# call this function will do nothing
IncludingFile

# Get-Foo is still not visible here.

```
This is what you can do.
```ps
. IncludingFile

Get-Foo # is visible here.

```

The base directory of dot sourcing is `Get-Location`.
