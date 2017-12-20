+++
title = "Introduction"
description = "Introduction"
date = "2017-04-24T18:36:24+02:00"

+++

OPRAmachine is an interactive web application designed to simplify the process of submitting a New Jersey Open Public Records Act (OPRA) request to state and local governmental agencies. OPRAmachine provides tracking functionality to ensure that your request is dealt with by public bodies in the time period prescribed by law. Each request that is made through the site is published on our website for all to see, allowing the entire public to benefit from each individual request that is made through the site.

### The OPRA request process on OPRAmachine

This diagram illustrates the lifecycle of a request for public records made via our web application.

{{<mermaid align="left">}}
graph LR;
    A[Requester submits initial request] -->|OPRA request delivered via email| B(Custodian receives request)
    B --> C{Records Custodian Responds}
    C -->|Request Approved| D[Documents Posted on OPRAmachine]
    C -->|Request Denied| E[Denial Letter Posted on OPRAmachine]
{{< /mermaid >}}
