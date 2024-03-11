**Definition:** 
 A markup language that defines rules for encoding documents in a format that is both human-readable and machine-readable.

A language and format used for storing and transmitting data.
A native file format used in Windows systems.
Consists of:
- Tags: used to store and identify data. Pairs that must contain a start tag and an end tag. `<tag>___</tag>`
- Elements: Elements include both the data contained inside of a tag and the tags itself. All XML entries must contain at least one root element. Root elements contain other elements that sit underneath them, known as child elements. E.G.
```
<Event> 
  <EventID>4688</EventID> 
  <Version>5</Version>
</Event>
```
- Attributes: Used to provide additional information about elements. Included as the second part of the tag & must always be quoted using either single or double quotes 
  E.G.
```
<EventData>
 <Data Name='SubjectUserSid'>S-2-3-11-160321</Data> 
 <Data Name='SubjectUserName'>JSMITH</Data>
 <Data Name='SubjectDomainName'>ADCOMP</Data>
 <Data Name='SubjectLogonId'>0x1cf1c12</Data>
 <Data Name='NewProcessId'>0x1404</Data>
</EventData>
```
  
  