# Expand Array as Parameter

Use the magic character **'@'**.
```PowerShell
Function Test($a, $b, $c){
    Write-Host $a
    Write-Host $b
    Write-Host $c
}

$arr = @(1,2,3)
```
When you run `Test $arr`, you will get
```PowerShell
1 2 3


```

When you run `Test @arr`, you will get
```PowerShell
1
2
3
```


