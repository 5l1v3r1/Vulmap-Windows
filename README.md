# vulmap-windows
Host-based local vulnerability scanner. Finds installed software on the host, asks their vulnerabilities to vulmon.com API and print vulnerabilities with available exploits. All found exploits can be downloaded by Vulmap.

Vulmap Windows is part of [Vulmap Local Vulnerability Scanners Project](https://github.com/vulmon/Vulmap-Local-Vulnerability-Scanners)
## Screenshots
![Screenshot from terminal](https://raw.githubusercontent.com/yavuzatlas/vulmap-windows/master/bir.jpg)

![Screenshot-2 from terminal](https://raw.githubusercontent.com/yavuzatlas/vulmap-windows/master/iki.jpg)

## Recommended Platform
Compatible with PowerShell v3 and higher


## Usage

Parameter              | Description
-----------------------| -------------
-DefaultMode           | Conducts a vulnerability scanning. Default mode.
-OnlyExploitableVulns  | Conducts a vulnerability scanning and only shows vulnerabilities that have exploits.
-DownloadExploit       | Downloads given exploit.
-DownloadAllExploits   | Scans the computer and downloads all available exploits.


### Examples

* Default mode. Conducts a vulnerability scanning:
```
PS> Invoke-Vulmap
```

* Conducts a vulnerability scanning and only shows vulnerabilities that have exploits:
```
PS> Invoke-Vulmap -OnlyExploitableVulns
```

* Downloads given exploit:
```
PS> Invoke-Vulmap -DownloadExploit EDB9386
```

* Scans the computer and downloads all available exploits:
```
PS> Invoke-Vulmap -DownloadAllExploits
```




