# About Dot Sourcing

Use `.` (dot sourcing) to include file. It will only be included in current scope. This means you cannot write a function to include a file, and use it outside this function. Because it only visible the function instead of the callilng context.

What you can do is to use another `.` to open the function also.

The base directory of dot sourcing is `Get-Location`.
