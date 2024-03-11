An instance when malicious script exists in the web page a browser loads

Document Object Model based Cross Site Scripting attack
Document Object Model represents the structure of a document as a tree of objects where each object corresponds to a part of the document such as elements, attributes and text. Web browsers use the DOM to render webpages and allow scripts to interact with the page after it has been loaded.

A malicious script can be seen in the URL
![[Pasted image 20231015192241.png]]
The URL contains parameter values that reflect input from the user (this site allows users to select colour themes)
![[Pasted image 20231015192358.png]]
In a DOM-based XSS attack criminals change the parameter that's expecting an input e.g. they could hide malicious JavaScript in the HTML tags and then the browser would process the HTML and execute the JavaScript