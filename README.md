This is the Good Standing Certificate System, whose components include:

- A web application with email validation, certificate validation and certificate form request
- A Government Messaging Queue API for requesting transactions be validated asynchronously with the Department of Justice and the Police Department as well as notifying users via email
- Asynchronous Workers that can process jobs and retry them using an exponential backoff strategy, should the underlying dependencies fail (such as agencies whose systems go offline or become unresponsive) 
