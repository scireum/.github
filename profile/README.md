![scireum GmbH](https://scireum.de/wp-content/uploads/2021/07/cropped-logo_scireum3-300x98.png)

> Die scireum GmbH entwickelt Softwareprodukte in den Bereichen Handelsinformationssysteme, E-Commerce und Messaging.


We're a software company located in Germany next to the city of Stuttgart. We're a firm believer in open source software and thus release as much as possible under accessible licenses.

[https://www.scireum.de](https://www.scireum.de)


## Java

Our language of choice for our SaaS platforms is **Java**. As we build 4 products which share a lot of functionality (all of them are multi-tenant / cloud native / SaaS platforms). We therefore built the [SIRIUS Framework](https://github.com/scireum/sirius-kernel) which provides dependency injection, database connectivity, cluster monitoring and maintenance, support for scheduling and work offloading on worker servers etc.

The framework is split into several libraries, depending on the functionality needed (to better control which dependencies are required):
* [SIRIUS kernel](https://github.com/scireum/sirius-kernel)
* [SIRIUS web](https://github.com/scireum/sirius-web)
* [SIRIUS db](https://github.com/scireum/sirius-db)
* [SIRIUS biz](https://github.com/scireum/sirius-biz)

We also (sadly) had to build a parser and compiler for SASS:
* [server-sass](https://github.com/scireum/server-sass)

Also, we built a simple parsing library (used by SIRIUS web for the **Tagliatelle Compiler** and by **server SASS**):
* [parsii](https://github.com/scireum/parsii)

Finally, we use SIRIUS to build a test-application, which we internally used to mock the API of S3:
* [S3 Ninja](https://github.com/scireum/s3ninja)

## JavaScript

Building web based products, we could not prevent the creation of some JS frameworks / libraries:

* [token-autocomplete](https://github.com/scireum/token-autocomplete)
* [CinematicJS](https://github.com/scireum/CinematicJS)

## Rust

We use **Rust** to offload memory and performance intense tasks from Java. We therefore built a runtime to provide ultra low-latency micro services via the **Redis RESP** protocol:
* [Jupiter](https://github.com/scireum/jupiter)
