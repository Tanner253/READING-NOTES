# AWS S3

- Scale storage resources to meet fluctating needs.
- store data across amazon classes to reduce cots without upfront investment
- protect your data
- easily manage data at scale with robust access controls.

an object storage service offering industry leading scalability with data availability, security, and performance. 
![Diagram](https://d1.awsstatic.com/s3-pdp-redesign/product-page-diagram_Amazon-S3_HIW.cf4c2bd7aa02f1fe77be8aa120393993e08ac86d.png)

## Lambda is...

- serverless computing service provided by amazon web services. users can create self contained functions and upload them to lambda to be called in a flexibable manner.
the main value of serverless is that computing refers to not needing to maintain your own server to run these select functions.

- When building Serverless applications, AWS Lambda is one of the main candidates for running the application code. Typically, to complete a Serverless stack you’ll need:

a computing service;
a database service; and
an HTTP gateway service.

- Due to Lambda’s architecture, it can deliver great benefits over traditional cloud computing setups for applications where:

individual tasks run for a short time;
each task is generally self-contained;
there is a large difference between the lowest and highest levels in the workload of the application.

![Diagram of lambda functions](https://d1.awsstatic.com/product-marketing/Lambda/Diagrams/product-page-diagram_Lambda-RealTimeFileProcessing.a59577de4b6471674a540b878b0b684e0249a18c.png)

### CDN 
[COPY AND PASTED FROM: THIS URL](https://cyberhoot.com/cybrary/content-delivery-network-cdn/)
A Content Delivery Network (CDN) is a geographically distributed group of servers that work together to provide fast delivery of Internet content. A CDN allows for the fast transfer of data needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos.

CDNs work through servers nearest to the website visitor respond to the request. The content delivery network copies the pages of a website to a network of servers that are spread out at geographically different locations, caching the contents of the page. When a user requests a webpage that is part of a content delivery network, the CDN will redirect the request from the originating site’s server to a server in the CDN that is closest to the user and deliver the cached content. CDNs will also communicate with the originating server to deliver any content that has not been previously cached. In turn, the speed is improved by distributing content closer to the website visitors by using a nearby CDN server, causing visitors to experience faster page loading times. In simpler terms, for example, instead of a user in London trying to access a server in LA, which can cause slower Internet speeds, the user would be redirected through a CDN that is geographically closest to them (London, Paris, Stockholm, etc). As of today, the majority of web traffic goes through through CDNs, including traffic from major sites like Facebook, Netflix, and Amazon.

Employing a CDN doesn’t only speed up the delivery of Internet content, it helps protect your website against certain forms of cyber attacks, such as Denial of Service attacks. It protects against these threats because CDNs allow for the handling of more traffic and withstanding hardware failure better than many origin servers. 