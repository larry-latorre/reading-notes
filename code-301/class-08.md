# APIs

## API Design Best Practices

**What does REST stand for?**

REST stands for Representational State Transfer. It is an architectural style for designing networked applications. REST is often used in the context of web services, where it provides a set of constraints that, when applied to the architecture of a web service, make it more scalable, maintainable, and uniform.

**REST APIs are designed around a ____.**

The "Uniform Interface" is one of the fundamental principles of RESTful design. It provides a standardized way to interact with resources through a consistent set of conventions. This includes the use of standard HTTP methods (GET, POST, PUT, DELETE), resource-based URIs (Uniform Resource Identifiers), and representations (such as JSON or XML) for data exchange.

**What is an identifier of a resource? Give an example.**

An identifier of a resource is a unique and unambiguous way to distinguish and locate a specific resource in a system. In the context of RESTful APIs, these identifiers are typically represented by URIs (Uniform Resource Identifiers).

**What are the most common HTTP verbs?**

The most common HTTP verbs (methods) are:

1. **GET:** Retrieves data from a specified resource. The GET request should not have a request body, and it is idempotent, meaning making the same request multiple times has the same effect as making it once.

2. **POST:** Submits data to be processed to a specified resource. It is non-idempotent, meaning making the same request multiple times might have different effects.

3. **PUT:** Updates a resource or creates a new resource if it does not exist at the specified URI. It is idempotent.

4. **DELETE:** Deletes the specified resource. It is idempotent.

5. **PATCH:** Applies partial modifications to a resource. It is typically used to update a resource with only the changes provided, rather than sending the complete resource representation. It is not guaranteed to be idempotent.

6. **OPTIONS:** Returns the HTTP methods that the server supports for the specified URL. This can be used by the client to discover the allowed methods for a resource.

7. **HEAD:** Similar to GET but does not return a message body. It is often used to retrieve metadata about a resource.

These HTTP methods provide a standardized way for clients to interact with resources on the web. They are a crucial part of the RESTful architectural style.

**What should the URIs be based on?**

URIs (Uniform Resource Identifiers) in RESTful APIs should be based on the resources and actions that the API exposes. The design of URIs is an important aspect of RESTful architecture, and they should reflect a clear and meaningful structure. Here are some guidelines:

1. **Resource-Centric:** URIs should be based on resources, representing the entities or objects that the API exposes. For example:
   - Good: `/users/123`
   - Avoid: `/getuser?id=123`

2. **Use Nouns for Resources:** URIs should use nouns to represent resources rather than verbs. Nouns convey the idea of entities, making the API more intuitive.
   - Good: `/products/456`
   - Avoid: `/getProductById/456`

3. **Use Plural Nouns:** Resource names in URIs should typically be plural to represent a collection of resources.
   - Good: `/users`
   - Avoid: `/user`

4. **Avoid Verbs in URIs:** Actions or operations should be expressed using HTTP methods (GET, POST, PUT, DELETE) rather than including verbs in the URIs.
   - Good: `POST /users` to create a new user
   - Avoid: `/createUser`

5. **Hierarchy and Nesting:** Use hierarchical structures in URIs to represent relationships between resources.
   - Good: `/departments/101/employees/789`
   - Avoid: `/employee?deptId=101&empId=789`

6. **Consistency:** Maintain consistency in URI naming conventions across the API to make it predictable for developers.

7. **Avoid Unnecessary Details:** URIs should focus on essential information. Avoid including implementation details or unnecessary information.
   - Good: `/orders/123`
   - Avoid: `/orders/123/details?includeItems=true`

By following these principles, URIs become more expressive, predictable, and user-friendly, contributing to the overall design and usability of the RESTful API.
**Give an example of a good URI.**

Certainly! Let's consider an example of a good URI based on the guidelines mentioned earlier. Suppose we have an e-commerce API dealing with products:

- **Resource:** Product
- **Use of Noun:** "products"
- **Plural Noun:** Represents a collection of products
- **Avoiding Verbs:** Actions are expressed using HTTP methods

Example of a Good URI:

```
GET /products            // Retrieves a list of all products
GET /products/123        // Retrieves details of a specific product with ID 123
POST /products           // Creates a new product
PUT /products/123        // Updates details of the product with ID 123
DELETE /products/123     // Deletes the product with ID 123
```

In this example:

- `/products` represents the collection of products.
- `/products/123` represents a specific product with ID 123.
- The HTTP methods indicate the actions performed on these resources.

This URI structure is clear, follows RESTful principles, and provides a meaningful representation of the resources and their actions within the e-commerce API.

**What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?**

A 'chatty' web API refers to an API that requires a large number of requests to perform a single operation or retrieve a specific set of data. In other words, it involves a high number of small, fine-grained requests to the server.

Whether having a 'chatty' web API is considered good or bad depends on various factors, including the context and requirements of the application. Here are some considerations:

**Pros of a Chatty API:**

1. **Granularity:** Chatty APIs often have a high level of granularity, allowing clients to request only the specific data they need. This can be beneficial for clients with limited bandwidth or devices with low processing power.

2. **Flexibility:** Fine-grained requests provide flexibility for clients to tailor their interactions with the API according to their specific needs.

**Cons of a Chatty API:**

1. **Performance Overhead:** Each HTTP request incurs overhead in terms of latency, network bandwidth, and server processing. With many small requests, the cumulative performance overhead can be significant.

2. **Increased Latency:** Multiple requests may result in higher latency, especially if the client needs to wait for the completion of each request before initiating the next one.

3. **Complexity:** Chatty APIs can lead to more complex client-side logic, as clients may need to manage multiple requests and responses to achieve a single operation.

**Recommendations:**

- **Consider Use Cases:** Evaluate the specific use cases and requirements of the application. For some applications, a chatty API might be suitable, while for others, a more coarse-grained approach might be preferable.

- **Batching:** If a chatty API is causing performance issues, consider implementing batch requests where multiple operations are bundled into a single request, reducing the overhead.

- **Caching:** Implement caching mechanisms to mitigate the impact of multiple requests for the same data.

In summary, whether a 'chatty' web API is good or bad depends on the specific needs of the application. It is essential to strike a balance between granularity and performance considerations, taking into account factors such as network conditions, client capabilities, and the overall user experience.
**What status code does a successful GET request return?**

A successful GET request typically returns a status code of `200 OK`. The HTTP status code 200 indicates that the request was successful, and the server has fulfilled the client's request by returning the requested resource.

In addition to `200 OK`, there are other success-related status codes that might be used in specific situations:

- `201 Created`: The request has been fulfilled, and a new resource has been created as a result of it. This status is often used for successful POST requests that result in resource creation.

- `204 No Content`: The server successfully processed the request but does not need to return a representation of the resource. It is commonly used for successful DELETE requests.

However, for a standard successful GET request, the `200 OK` status code is the most commonly used.
**What status code does an unsuccessful GET request return?**

An unsuccessful GET request typically returns a status code in the 4xx or 5xx range. The specific status code depends on the nature of the error. Here are some common status codes for unsuccessful GET requests:

1. **400 Bad Request:** The server cannot process the request due to a client error, such as malformed request syntax or invalid request message framing.

2. **401 Unauthorized:** The request requires user authentication. The client must provide valid credentials to access the requested resource.

3. **403 Forbidden:** The server understood the request, but it refuses to authorize it. The client does not have the necessary permissions to access the resource.

4. **404 Not Found:** The server cannot find the requested resource. This is a common response for situations where the requested URI does not correspond to an existing resource.

5. **405 Method Not Allowed:** The method specified in the request (e.g., GET) is not allowed for the specified resource.

6. **406 Not Acceptable:** The server cannot produce a response matching the list of acceptable values defined in the request's headers.

7. **408 Request Timeout:** The server timed out while waiting for the request. The client may retry the request.

8. **429 Too Many Requests:** The client has sent too many requests in a given amount of time ("rate limiting").

These are just a few examples, and there are other status codes that might be applicable in different scenarios. The choice of status code provides information about the nature of the error, helping clients understand and respond appropriately.
**What status code does a successful POST request return?**

A successful POST request typically returns a status code of `201 Created` or `200 OK`, depending on the specific circumstances and conventions of the API.

1. **201 Created:** This status code indicates that the request has been fulfilled, resulting in the creation of a new resource. It is commonly used to signal that a POST request has successfully created a resource on the server.

   Example:
   ```
   HTTP/1.1 201 Created
   Location: /resources/new-resource
   ```

2. **200 OK:** In some cases, a server might respond with a `200 OK` status code for a successful POST request. This is acceptable, especially if the response body contains details about the newly created resource.

   Example:
   ```
   HTTP/1.1 200 OK
   Content-Type: application/json

   {
     "id": 123,
     "name": "New Resource"
   }
   ```

While `201 Created` is more specific for indicating resource creation, some APIs might use `200 OK` for consistency with other successful responses.

It's essential to check the API documentation to understand how it handles successful POST requests and which status code it uses in such cases.

**What status code does a successful DELETE request return?**

A successful DELETE request typically returns a status code of `204 No Content`. The `204` status code indicates that the server has successfully processed the request, but there is no content to send in the response body.

Here is an example of a successful DELETE response:

```
HTTP/1.1 204 No Content
```

In this case, the absence of a response body with content (such as JSON or XML) is a characteristic of the `204 No Content` status. The status code signals that the resource has been successfully deleted, and there is no additional information to include in the response body.

It's worth noting that some APIs might choose to return a `200 OK` status code instead of `204 No Content` for a successful DELETE request, especially if they include additional information about the deleted resource in the response body. However, using `204 No Content` is a common and appropriate practice for indicating the success of a DELETE operation.