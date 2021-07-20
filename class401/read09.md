# WRRC and Java

## The HTTP Request Lifecycle 

**Step 1: Local Processing**<br>
***Depending on how in depth you want to get, much can happen during this step depending on the application making the request.***

**Step 2: Resolve an IP**<br>
***Like the processing done locally, resolving an IP from a "DNS server"2 is a sequence that includes many steps, and includes failovers if the first request fails to return an address.***

**Step 3: Establish a TCP Connection**<br>
***Since the request is sent over TCP6, which is a transport layer protocol like UDP, the client must open a TCP connection.***

**Step 4: Send an HTTP Request**<br>

**Step 5: Tearing Down and Cleaning Up**

## Do a Simple HTTP Request in Java

- **Creating a Request**<br>
***We can create an HttpUrlConnection instance using the openConnection() method of the URL class. Note that this method only creates a connection object but doesn't establish the connection yet.***

- **Adding Request Parameters**<br>
***If we want to add parameters to a request, we have to set the doOutput property to true, then write a String of the form param1=value¶m2=value to the OutputStream of the HttpUrlConnection instance.***

- **Setting Request Headers**<br>
***Adding headers to a request can be achieved by using the setRequestProperty() method.***

- **Configuring Timeouts**<br>
***HttpUrlConnection class allows setting the connect and read timeouts. These values define the interval of time to wait for the connection to the server to be established or data to be available for reading. To set the timeout values, we can use the setConnectTimeout() and setReadTimeout() methods***

- **Handling Cookies**<br>
***The java.net package contains classes that ease working with cookies such as CookieManager and HttpCookie. to read the cookies from a response, we can retrieve the value of the Set-Cookie header and parse it to a list of HttpCookie objects.***

- **Handling Redirects**<br>
***We can enable or disable automatically following redirects for a specific connection by using the setInstanceFollowRedirects() method with true or false parameter.***

- **Reading the Response**<br>
***Reading the response of the request can be done by parsing the InputStream of the HttpUrlConnection instance. To execute the request, we can use the getResponseCode(), connect(), getInputStream() or getOutputStream() methods.***

- **Reading the Response on Failed Requests**<br>
***If the request fails, trying to read the InputStream of the HttpUrlConnection instance won't work. Instead, we can consume the stream provided by HttpUrlConnection.getErrorStream().***