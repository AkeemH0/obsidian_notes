A log format that uses key-value pairs to structure data and identify fields and their corresponding values. Contains the following fields: 
`CEF:Version|Device Vendor|Device Product|Device Version|Signature ID|Name|Severity|Extension`
Fields are separated by | (pipe) but Anything in the extension part must be written in key-value format with no |
[[Syslog]] is a common method to transport logs like CEF
E.G. This log entry contains details about a ***Security*** application called ***threat manager*** that ***successfully stopped a worm*** from spreading from the internal network ***10.0.0.2*** to the external network ***2.1.2.2*** through the ***port 1232***. High severity level of ***10***.
`Sep 29 08:26:10 host CEF:1|Security|threatmanager|1.0|100|worm successfully stopped|10|src=10.0.0.2 dst=2.1.2.2 spt=1232`
Fields:
- **Syslog Timestamp**: Sep 29 08:26:10    
- **Syslog Hostname**: host
- **Version**: CEF:1    
- **Device Vendor**: Security
- **Device Product**: threatmanager
- **Device Version**: 1.0
- **Signature ID**: 100
- **Name**: worm successfully stopped
- **Severity**: 10
- **Extension**: contains data written as key-value pairs. Optional.
  