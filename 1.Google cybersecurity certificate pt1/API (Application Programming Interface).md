**Definition:**
 A set of protocols and tools for communication between software applications, enabling them to interact and share data with each other.

An interface that enables different software systems and applications to communicate and interact with each other, sharing data and functionality securely.
A set of rules that define how software components interact with each other.

APIs are often used to tasks like authentication where different systems verify the identity of users or applications accessing their services.

Security measures
- Utilize secure protocols such as HTTPS (encrypt data in transit) for network communication
- Require [[Authentication]] and [[Authorization]] often throughout [[API tokens, API credentials]]([[Tokenization]])
- [[Network segmentation]]: APIs and microservices and software components are usually deployed in isolated networks or segments which have a distinct access point [[API gateway]].
- [[API gateway]] secure gateways for accessing the API. Perform authentication, authorization, [[Access control]]s, traffic management & encryption, [[Load balancing]]
- encrypt data at rest ([[FDE (Full-disk Encryption)]])

*Imagine you're at a library (your computer) and want a book (data) from the librarian (server). The librarian doesn't bring the whole bookshelf; instead, you use a request slip (API call) to get the specific book you need. Just like the slip ensures you get the right book, APIs ensure the right data is exchanged between software without revealing everything. Securing the process is like making sure only authorized people can use the request slips.*