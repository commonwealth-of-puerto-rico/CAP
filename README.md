This is the Good Standing Certificate System ("Servicio para el Certificado de Antecedentes Penales" in Spanish), whose components include:

- A web application with email validation, certificate validation and certificate form request
- A Government Messaging Queue API for requesting transactions be validated asynchronously with the Department of Justice and the Police Department as well as notifying users via email
- Asynchronous Workers that can process jobs and retry them using an exponential backoff strategy, should the underlying dependencies fail (such as agencies whose systems go offline or become unresponsive)

The production instance of the Good Standing Certificate System is served from https://servicios.pr.gov/cap

To learn more about this project, see this technical presentation:
<a href="http://www.slideshare.net/AndrsColnPrez/good-standing-certificate-knowledge-transfer-presentation-by-andres-colon">Building Modern Digital Services on Scalable Private Government Infrastructures using Open Source Technologies for Public Service</A>
