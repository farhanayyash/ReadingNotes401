# The HTTP Request Lifecycle

## Step 1: Local Processing
 This step depending on the application making the request.  I am going to proceed on the understanding this request is being made by a browser.
- our browser extracts the "scheme"/protocol (we have established
that this will be HTTP), host.
- Now that the browser has the intended hostname for the request, it needs to resolve an IP address.

## Resolve an IP
- Your request will now have to travel many network devices to reach its target DNS server.
- Once your request arrives at your configured DNS server, the server looks for the address associated with the requested hostname.

## Establish a TCP Connection
### TCP and UDP
One of the key differences between TCP and UDP is that TCP ensures delivery and ordered data transmission. Much of this is done very simply, using what’s known as a sequence number for every byte sent. This allows the receiver to re-order received packets back into their original order and allows the sender to retransmit any packet that does not get acknowledged by the receiver.

## Send an HTTP Request

## How to performing HTTP requests in Java
- HttpUrlConnection
The HttpUrlConnection class allows us to perform basic HTTP requests without the use of any additional libraries. All the classes that we need are part of the java.net package.

## Creating a Request
We can create an HttpUrlConnection instance using the openConnection() method of the URL class

## Adding Request Parameters
If we want to add parameters to a request, we have to set the doOutput property to true, then write a String of the form param1=value¶m2=value to the OutputStream of the HttpUrlConnection instance

## Reading the Response
Reading the response of the request can be done by parsing the InputStream of the HttpUrlConnection instance.

To execute the request, we can use the getResponseCode(), connect(), getInputStream() or getOutputStream() methods