### **200 OK**
- **Category:** Success
- **Description:** This status code indicates that the request has succeeded. The meaning of the success depends on the HTTP method:
  - **GET:** The resource has been fetched and is transmitted in the response.
  - **POST:** The resource has been created, and the response includes information about the created resource.
  - **PUT/PATCH:** The resource has been updated successfully.
  - **DELETE:** The resource has been deleted successfully.
  
  **Example Usage:** A successful request for a web page or API call will return a 200 status.

---

### **400 Bad Request**
- **Category:** Client Error
- **Description:** This status code indicates that the server could not understand the request due to invalid syntax. It tells the client that there was an error in the request that prevents it from being processed. This could be caused by missing parameters, incorrect data format, or malformed headers.
  
  **Example Usage:** Sending an incomplete or incorrect API request without required parameters, or with improperly formatted data.

---

### **401 Unauthorized**
- **Category:** Client Error
- **Description:** This status code means that the request has not been applied because it lacks valid authentication credentials. It implies that the client must authenticate itself to get the requested response. The server may return this code when the request requires authentication, such as accessing a protected resource, but the user has not logged in or provided valid credentials.
  
  **Example Usage:** Attempting to access a restricted page or API endpoint without providing the necessary API key or login credentials.

---

### **403 Forbidden**
- **Category:** Client Error
- **Description:** This status code indicates that the server understands the request but refuses to authorize it. Even though the request is valid, the server will not allow it to be processed due to insufficient permissions, such as trying to access a resource that the current user does not have permission to view or modify.
  
  **Example Usage:** Trying to access a file or resource on the server for which the user doesn't have the correct permissions, even though they are authenticated.

---

### **404 Not Found**
- **Category:** Client Error
- **Description:** This status code is one of the most common, indicating that the server cannot find the requested resource. It suggests that either the resource has been moved, deleted, or was never present. The server could also return this response if the URL is incorrect.
  
  **Example Usage:** Visiting a URL on a website that does not exist, or making an API call to an endpoint that is not available.

---

### **500 Internal Server Error**
- **Category:** Server Error
- **Description:** This status code signifies that the server encountered an unexpected condition that prevented it from fulfilling the request. It’s a generic error message, meaning the server has encountered an error, but the exact nature of the issue is not specified. It’s typically caused by server misconfigurations, bugs in server-side software, or resource limitations.
  
  **Example Usage:** A bug in the server-side code causes it to fail, like a missing database connection or an error in business logic during processing.

---

### **502 Bad Gateway**
- **Category:** Server Error
- **Description:** This status code indicates that the server, while acting as a gateway or proxy, received an invalid response from the upstream server it needed to access in order to fulfill the request. This can happen if the upstream server is down or not responding correctly.
  
  **Example Usage:** If a web server acts as a reverse proxy and tries to forward requests to an application server that is down or malfunctioning, a 502 error is returned.

---

### **503 Service Unavailable**
- **Category:** Server Error
- **Description:** This status code means the server is currently unable to handle the request, typically due to temporary overloading or maintenance. It suggests that the issue is temporary, and the client should try again later.
  
  **Example Usage:** The server is undergoing maintenance or is temporarily overloaded, causing it to be unable to process requests at the moment.
