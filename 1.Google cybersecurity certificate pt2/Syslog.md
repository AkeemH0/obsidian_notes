PORT 514 UDP
A standard for logging and transmitting data. Can be used to refer to any of its three capabilities:
- Syslog Protocol: 
  Used to transport logs to a centralized log server for log management. Uses port 514 for plaintext logs and port 6514 for encrypted logs.
- Syslog Service: 
  Acts as a log forwarding service that consolidates logs from multiple sources into a single location. Works by receiving and then forwarding any syslog log entries to a remote server.
- Syslog Log format: 
  One of the most commonly used log formats. Native logging format used in Unix systems. Consists of three components: header, structured-data & message.
 E.G.
 `<236>1 2022-03-21T01:11:11.003Z virtual.machine.com evntslog - ID01 [user@32473 iut="1" eventSource="Application" eventID="9999"] This is a log entry!`

 [[Header]]: 
  - Timestamp: `2022-03-21T01:11:11.003z`
  - Hostname: `virtual.machine.com`
  - Application: `evntslog`
  - Message ID: `ID01

 Structured-data:
  contains additional logging information enclosed in square brackets and structured in key-value pairs.
  `[user@32473 iut="1" eventSource="Application" eventID="9999"]`

 Message: 
 Contains detailed log message about the event E.G. `This is a log entry!`
 
 Priority (PRI): indicates the urgency of the logged event & is contained with angle brackets <>. E.G. `<236>`. The lower the priority number the more urgent the event is

  