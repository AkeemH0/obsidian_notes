Searches through data that has been ingested, parsed and normalized.
Retrieves results faster than a [[Raw log search]] because it searches through indexed and structured data.
Common fields:
 - Entities/nouns: Provides additional context about the device, user or process that's involved in an event. E.G. hostname, username & IP address .
 - Event metadata: A basic description of an event, including what type of event it is & timestamp etc..
 - Network metadata: Provides information about network-related events and protocol details.
 - Security results: Provides the security-related outcome of events. E.G. an antivirus software detecting and quarantining a malicious file by reporting "virus detected and quarantined"

Example:
 `metadata.event_type = “USER_LOGIN” ` 
 - UDM search that uses the event metadata field to locate events relating to user logins
 - This UDM field `metadata.event_type` contains information about the event type. This includes information like timestamp, network connection, user authentication, and more. Here, the event type specifies `USER_LOGIN`, which searches for events relating to authentication.