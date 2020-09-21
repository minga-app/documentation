# Our technologies

## apps
We use the open source framework flutter to create fast cross-platform apps for iOS, Android and Desktop.  
State management is done with the BloC library.

## web
We implement a very rudimentary version of our app with AngularDart.

## shared code
We write all of our data models and logic in Dart, which are shared between backend, web and mobile apps.

## backend
We use Firebase Cloud Functions, which are written in Dart and then compiled to nodejs.

## database & storage
- We use Firebase Cloud Firestore for storing data.
- For media assets, we use Cloudinary.

# Future stack
Although Firebase is great for commercial projects or to see results fast, we try to become more vendor-independent and want to adjust our stack more towards **open standards**.  

- Cloud Firestore should be replaced by an open-source alternative.
- We plan to rewrite our backend with grpc-based microservices, so users don't write directly to the database but to the grpc endpoint.
- Client libraries for the grpc-API can be automatically generated in different languages (see [language support](https://en.wikipedia.org/wiki/Protocol_Buffers#Language_support)), which lowers the barrier for other people to build on our platform.
- All of the backend should be based on Docker and Kubernetes for orchestration, so it can easily be deployed on many of the big cloud providers or *own servers*.

**but why?**  
We want to be independent of corporate politics and the availability of their products.  
For example GCP is [blocked in some countries](https://support.google.com/a/answer/2891389?hl=en#:~:text=G%20Suite%20is%20available%20in,Korea%2C%20Sudan%2C%20and%20Syria.).
