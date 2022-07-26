![scireum GmbH](https://scireum.de/wp-content/uploads/2021/07/cropped-logo_scireum3-300x98.png)



We're a software company located in Germany next to the city of Stuttgart. We're a firm believer of open source software and thous release as much as possible under accessible licenses.

[https://www.scireum.de](https://www.scireum.de)

> Die scireum GmbH entwickelt Softwareprodukte in den Bereichen Handelsinformationssysteme, E-Commerce und Messaging.

## Java

Our language of choice for our SaaS platforms is **Java**. As we build 4 products which share a lot of functionality (all of them are multi-tenant / cloud native / SaaS platforms). We therefore built the [SIRIUS Framework](/scireum/sirius-kernel) which provides dependency injection, database connectivity, cluster monitoring and maintenance, support for scheduling and work offloading on worker servers etc.

The framework is split into several libraries, depending on the functionality needed (to better control which dependencies are required):
* [SIRIUS kernel](/scireum/sirius-kernel)
* [SIRIUS web](/scireum/sirius-web)
* [SIRIUS db](/scireum/sirius-db)
* [SIRIUS biz](/scireum/sirius-biz)

## JavaScript

Building web based products, we could not prevent the creation of some JS frameworks / libraries:

* [token-autocomplete](/scireum/token-autocomplete)
* [CinematicJS](/scireum/CinematicJS)

## Rust

We use **Rust** to offload memory and performance intense tasks from Java. We therefore built a runtime to provide ultra low-latency micro services via the **Redis RESP* protocol:
* [Jupiter](/scireum/jupiter)
