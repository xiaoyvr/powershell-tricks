# About ScriptBlock

Use & to execute it. Use param to define args just like functions.

If sometime you cannot get the correct behavior for a piping output, use a scriptblock to wrap and execute it.

```
& { & xunit.runner.exe "test.dll" } | Output-Default
```
