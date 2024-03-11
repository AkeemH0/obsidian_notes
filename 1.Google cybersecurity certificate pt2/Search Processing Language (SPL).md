Splunk's query language
Used to search and retrieve indexes using Splunk's Search & Reporting app
Utilises [[piping]] | 

`index=main fail *| chart count by host`

 - `index=main fail` This is the beginning of the search command that tells Splunk to retrieve events from an  index named main for events containing the search term fail. 
   
 - `*` The Asterix is a wildcard representing any character, telling Splunk to search for anything containing the previous term + any ending e.g. failure, failed, failing etc.

 - `|` The pipe character separates and chains the two commands index=main and chart count by host. This means that the output of the first command index=main is used as the input of the second command chart count by host. 
 
 - `chart count by host` This command tells Splunk to transform the search results by creating a chart according to the  count or number of events. The argument by host tells Splunk to list the events by host, which are the names of the devices the events come from. This command can be helpful in identifying hosts with excessive failure counts in an environment.

`""` specify a search for an exact string/phrase

The host field specifies the name of a host, such as a network device or other system, from which an event originates.
The source field identifies the file name from which an event originates