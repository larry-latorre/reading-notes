# REST

## What Google Learned From Its Quest to Build the Perfect Team

**To what extent did psychological safety impact your previous work experience?**

**How does this article inform your approach to working with others moving forward?**

Prioritizing Psychological Safety

Encouraging Open Communication

Supporting Risk-Taking

Continuous Improvement

**Who is Roy Fielding?**

Roy Fielding is a computer scientist renowned for his work on the Representational State Transfer (REST) architectural style. His 2000 doctoral dissertation, "Architectural Styles and the Design of Network-based Software Architectures," introduced REST, which has become a fundamental approach in the design of web services and APIs. Fielding's contributions have had a profound impact on web development practices, and he is recognized for his influential role in shaping the architecture of the World Wide Web. Additionally, he has been associated with the University of California, Irvine, and has played a key role in web standards and practices.

**Why don’t the techniques that we use in this class work well when we need to be able to talk to all of the machines in the world?**

The challenges include scalability issues, the complexity of global networks, latency due to physical distance, security and privacy concerns, diversity in devices and protocols, regulatory and legal considerations, and resource constraints. To address these challenges, global-scale technologies and protocols must prioritize scalability, resilience, and adaptability to accommodate the diverse and complex nature of worldwide communication.

**What is the HTTP protocol that Fielding and his friends created?**

Roy Fielding did not create the HTTP protocol; however, he played a crucial role in its development through his contributions to the World Wide Web Consortium (W3C) and the Internet Engineering Task Force (IETF). HTTP, or Hypertext Transfer Protocol, is the foundation of data communication on the World Wide Web, facilitating the transfer of hypertext resources between clients (such as web browsers) and servers. Fielding's notable contribution lies in his introduction of the Representational State Transfer (REST) architectural style in his doctoral dissertation, which has influenced the design principles of HTTP and web services, emphasizing key concepts like statelessness and a uniform interface.

**What does a GET do?**

The GET method in HTTP is used for retrieving data from a specified resource, typically a web server. It is considered "safe" and "idempotent," meaning it should not cause side effects, and multiple identical requests have the same effect as a single request. Data is sent as query parameters in the URL, making it visible in the address bar and suitable for sharing or bookmarking. GET requests can be cached for performance improvement, and they are commonly used for navigating through websites by following links or bookmarking pages.

**What does a POST do?**

The POST method in HTTP is used for submitting data to a specified resource, such as a web server. It involves sending data in the request body as key-value pairs, making it suitable for handling sensitive information. Unlike the GET method, which appends data to the URL, POST keeps data out of the visible URL. It is considered more secure for transmitting confidential information and is commonly used for actions that may cause side effects, such as form submissions. The POST method is crucial for scenarios where data needs to be submitted for processing on the server.

**What does PUT do?**

The PUT method in HTTP is used to either create a new resource or update an existing one at a specified URI. It is an idempotent operation, meaning multiple identical requests have the same effect as a single request. Data is sent in the request body, typically in JSON or another format, and the specified URI indicates the location where the resource should be stored or updated. Unlike POST, which is more general-purpose for data submission, PUT is specifically designed for resource creation or update operations.

**What does PATCH do?**

The PATCH method in HTTP is used to apply partial modifications to a resource. It allows clients to specify changes or updates to a resource without requiring the entire resource to be sent. PATCH requests are idempotent, meaning multiple identical requests have the same effect as a single request. Data for the partial update is sent in the request body, typically in JSON or another format, and the specified URI indicates the location of the resource to be partially updated. PATCH is particularly useful when making incremental changes to a resource without transmitting the entire data set.

### API Keys

Request a personal API key from the following APIs. You should receive these in your email within a few hours, often within minutes. Please request these keys prior to lecture to allow adequate time because you will need them in order to complete your lab assignment. Note: do not post your API keys in the Canvas discussion or on GitHub. Save them in a secure place.

### Geocoding API

**Did you get your API key?**

yes

### Weather Bit API

**Did you get your API key?**

yes

## Yelp API Docs

**Did you get your API key?**

yes

### The Movie DB API Docs

**Did you get your API key?**

yes
