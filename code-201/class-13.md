# Local Storage and How To Use It On Websites

**Why would a developer use local storage for a web application?**

 
 Local storage is a valuable tool for web developers. It is a fast, offline-capable, and easy-to-use way to store data that needs to persist between browser sessions. However, it is important to use local storage responsibly and to only store data that is not sensitive.

**What information should not be stored in local storage?**

Passwords: Passwords should always be stored on the server, not in the browser. If you need to store user passwords locally, you should use a secure hashing and encryption algorithm.

Credit card information: Credit card information should also be stored on the server, not in the browser. This is because credit card information is highly sensitive and can be easily used for fraud if it is stolen.

Personally identifiable information (PII): PII, such as names, addresses, and phone numbers, should also be stored on the server, not in the browser. This is because PII is sensitive information that can be used to identify and track individuals.

Authorization tokens: Authorization tokens are used to identify users on a web application. They should be stored on the server, not in the browser. This is because authorization tokens are valuable to attackers and can be used to impersonate users on the application.

Financial information: Financial information, such as account numbers and balances, should not be stored in local storage. This is because financial information is highly sensitive and can be used to steal money from users.

**Local storage can store what type of data?**

Local storage cannot store data without converting it to a string representation.

**How would you convert it to that type before storing?**

The specific method for converting data to a string before storing it in local storage will depend on the data type. However, the general process is to use a serialization technique to convert the data into a string representation that can be stored and later deserialized back into its original format.

For example, to convert an object to a string, you can use the JSON.stringify() method:

const obj = {
  name: "John Doe",
  age: 30,
  occupation: "Software Engineer"
};

const jsonString = JSON.stringify(obj);
console.log(jsonString); // Output: {"name":"John Doe","age":30,"occupation":"Software Engineer"}

