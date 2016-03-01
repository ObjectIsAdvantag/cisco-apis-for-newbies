# Everything programmable at Cisco

This guide is a opinionated tentative to synthesize [Cisco APIs for developers & ITPros](https://developer.cisco.com/site/devnet/index/) with No to little knowledge of Cisco hardware and software products.
Started as a tribute to my "First Days Party" at Cisco Live Berlin Feb 15-19th 2016.
Contributors welcome, CC BY 4.0 license.

- [New to Cisco APIs](#toc_DevNet)
- [Collaboration](#toc_Collaboration): [Spark](#toc_Spark), [Tropo](#toc_Tropo), [WebEx](#toc_WebEx)
- [Data & Analytics](#toc_Data)
- [DevOps, Software Tools & Automation](#toc_DevOps)
- [IoT](#toc_IoT)
- [Programmable infrastructure](#toc_ProgrammableInfrastructure)


# <a name="toc_DevNet"></a>New to Cisco APIs ?

You should definitely start with the [DevNet portal](https://developer.cisco.com/site/devnet/home/index.gsp), the one-stop for all development related activities with/to/from/above Cisco technologies.

Take a few minutes to create your account, it's really worth it :
- [DevNet](https://developer.cisco.com/site/devnet/home/index.gsp): umbrella to technical resources about IoT, Cloud Offerings, Progrommable Networks, Private & Hybrid cloud automation, Collaboration, BigData & Analytics, DevOps, DevOps, Microservices, Security
- [Learning labs](https://learninglabs.cisco.com/springboards) : step by step walkthroughs for ITPros & developers, featuring live environments to interact with Cisco programmable products
- [Programming foundation](https://learninglabs.cisco.com/modules/programming-found) : learn REST principles and how to call them via a User Interface, from the command line, or from code
- [Sandbox](https://developer.cisco.com/site/devnet/sandbox/): provision various CISCO hardware and network topologies and experiment Live APIs. Environments are provisionned for your own use from 3 hours to 7 days. APIC-EM , Cisco Open SDN Controller , Jabber , Webex , Intercloud Fabric...
- [DevNet Labs](https://developer.cisco.com/site/devnetlabs/) : Showcase of software projects built out of Cisco APIs and open technologies contributed by Cisco

# <a name="toc_Collaboration"></a>Collaboration

## <a name="toc_Tropo"></a>Tropo

Since 2009, [Tropo](http://www.tropo.com) provides Cloud Services to integrate SMS & Calls into your apps, and by integration, understand both ways :
your app can interact with incoming calls AND place outgoing calls, your app can send SMS messages AND take action at incoming SMS messages.
Worldwide availability, numbers in 42 countries, 80 speech languages
Data center facilities in the US, [coming to Europe by June 2016](https://medium.com/@ObjectIsAdvantag/cisco-tropo-is-coming-to-europe-in-spring-2016-add-sms-phone-calls-to-your-app-starting-today-b649a30a01e1)

- [Tropo APIs](https://www.tropo.com/docs/) : scripting, Web API & REST API documentation
- [Github Samples](https://github.com/tropo/tropo-samples)
- [DevNet Learning Lab](https://learninglabs.cisco.com/lab/tropo-intro/step/1) : integrate SMS & Calls into your apps, and by integration, understand both ways : your app can interact with incoming calls AND place outgoing calls, your app can send SMS messages AND take action at incoming SMS messages.
- [Pricing](https://www.tropo.com/pricing/)
- [Twitter](https://twitter.com/Tropo)
   - [changes](https://twitter.com/tropochanges) : Follow to see what [changes](changes.tropo.com) get made to Tropo
   - Technical team
      - [adam](https://twitter.com/akalsey)
      - [diggz](https://twitter.com/JohnnyDiggz)
      - [marcello](https://twitter.com/marchfederico)
      - [paul](https://twitter.com/paultodwyer)
      - [phil](https://twitter.com/PBellanti)


## <a name="toc_Spark"></a>Cisco Spark

Since March 2015, [Cisco Spark](https://www.ciscospark.com/) is the all-in-one Cloud Collaboration platform for the extended enterprise.
In short, Cisco Spark is a multi-client platform (Phone, Mac, Windows apps), backed by Cloud Collaboration Services (persistent chat rooms, WebRTC video conferencing), enabling 1-1, 1-few, 1-many communication.
Cisco Spark can be used for short-live meeting rooms, but also long-live collaborative workspaces, opened to internal co-workers, but also partners and external communities.

The overall Cisco Spark platform can be managed via [REST APIs](https://developer.ciscospark.com/getting-started.html) : easily bring messaging capabilities into your apps, automatically send messages to Spark rooms based on real-world/business events.

- [Spark APIs](https://developer.ciscospark.com/getting-started.html): REST APIs interactive documentation
- [Spark for developers](https://developer.cisco.com/site/spark/): the DevNet umbrella for all Spark related contents for developers
- [Learning labs](https://developer.cisco.com/site/spark/): Rooms and messages, Authentication, WebHooks
- [Twitter](https://twitter.com/ciscosparkdev)
   - Technical team
      - [adam](https://twitter.com/akalsey)
      - [diggz](https://twitter.com/JohnnyDiggz)
      - [marcello](https://twitter.com/marchfederico)
      - [paul](https://twitter.com/paultodwyer)
      - [phil](https://twitter.com/PBellanti)
   - Consulting team
      - [Fabien Medat](https://www.ciscospark.com/): head of technical consulting for Collaboration French Team

## <a name="toc_WebEx"></a>WebEx

- [WebEx APIs](https://developer.cisco.com/site/webex-developer/develop-test/try-webex-apis/)
- [DevNet Sandbox](https://developer.cisco.com/site/devnet/sandbox/available-labs/comm-collab/) : explore Cisco WebEx API capabilities and start developing your proof-of-concept solution
- [WebEx Developer Program](https://developer.cisco.com/site/webex-developer/web-conferencing/program-benefits/)


# <a name="toc_Data"></a>Data & Analytics

## PANDA

https://developer.cisco.com/site/panda/

## Cisco Zeus (Cloud offering, Restricted Beta)

Zeus is a Cloud-based Logging and Monitoring Service. Use the Zeus API or standard agents (such as fluent, syslog, logstash, collectd, statsd) to push your logs and metrics to Zeus.
Interactively visualize, search or analyze your data, or query / aggregate via the Zeus API.

- [Zeus Portal](http://www.ciscozeus.io/) : request access to the beta
- [Github Repo](https://github.com/CiscoZeus) : python , ruby, java and go clients
- [API Documentation](http://api.ciscozeus.io/) : Swagger UI
- [Getting started guide](http://blogs.ciscozeus.io/2015/09/getting-started-with-logs-and-metrics.html)
- [Zeus Blog](http://blogs.ciscozeus.io/


# <a name="toc_DevOps"></a>DevOps, Software Tools & Automation

## DevOps

### Cisco Shipped (Cloud offering, Public Beta)

Shipped is a CI and CD platform, built on top of best of breed technologies and opensource projects : Docker, Vagrant, Drone (a Continuous Delivery platform built on Docker, written in Go) and MANTL.

Shipped can deploy your code on any MANTL capable platforms: either run by Cisco Cloud or in your own datacenter.

- [Shipped Portal](https://ciscoshipped.io/)
- [DevNet Zone](https://developer.cisco.com/site/shipped/)
- [Documentation](https://ciscoshipped.io/shipped/api-docs/build/index.html)
- [Walkthroughs](https://ciscoshipped.io/shipped/api-docs/build/index.html#walkthroughs) : setup a project, build, deploy
- [Twitter](https://twitter.com/projectshipped)


## Microservices

### MANTL (opensource, v1.0)

MANTL reached version 1.0 in February 2016.

- [MANTL](https://mantl.io/) : a microservices framework on top of openstack


## Web frameworks

### NeXt

The NeXt javascript framework presents network topologies via user friendly Web interactions. NeXt can display large and complex network topologies, aggregated network nodes,  traffic/path/tunnel/group visualizations and includes several layout algorithms, map overlays, and preset user friendly interactions.

- [NeXt Portal](https://developer.cisco.com/site/neXt/)
- [OpenDayLight Project Page](https://wiki.opendaylight.org/view/NeXt:Main) : NeXt can work together with the [OpenDayLight User Interface - DLUX](https://nexus.opendaylight.org/content/sites/site/org.opendaylight.docs/master/userguide/manuals/userguide/bk-user-guide/content/_working_with_dlux.html)


# <a name="toc_IoT"></a>DevOps, Software Tools & AutomationIoT


# <a name="toc_ProgrammableInfrastructure"></a>Programmable infrastructur

[DevNet Networking Portal](https://developer.cisco.com/networking): All about Cisco networking technologies for developers

## Configure your network

- [RESTCONF](http://sdntutorials.com/what-is-restconf) : HTTP-based protocol, which provides REST-like APIs to manipulate YANG modeled data and invoke YANG modeled RPCs, using XML or JSON as payload format

- [NETCONF]() : XML-based RPC protocol, which provides abilities for client to invoke YANG-
modeled RPCs, receive notifications and to read, modify and manipulate YANG modeled data.

- [Cisco Prime Infrastructure API](https://developer.cisco.com/site/prime-infrastructure/documents/api-reference/api-reference/)

- ACI/APIC

## Software Defined Network (SDN) & Network Functions Virtualization (NFV)

### OpenDayLight

[OpenDaylight](https://www.opendaylight.org/) aims to make interoperable and programmable networks a reality, by delivering the benefits of Software Defined Networks (SDN) and Network Functions Virtualization (NFV) to networks of any size and scale. [Use cases](https://www.opendaylight.org/use-cases/) include Automated / Agile / OnDemand Service Delivery and Dynamic Network Resources Optimization.

[How ?](https://www.opendaylight.org/platform-overview-beryllium) with SDN, you can achieve network programmability and abstraction, but then comes the question of managing it. Via common API frameworks, OpenDayLight helps create abstractions North or South of the controller without having to look under the hood. Several  intent and policy approaches to do this include ALTO, Group Based Policy and Network Intent Composition.

Architecture: OpenDayLight employs a model-driven approach to describe the network, the functions to be performed on it and the resulting state or status achieved.
- by sharing YANG data structures in a common data store and messaging infrastructure, OpenDaylight allows for fine-grained services to be created then combined together to solve more complex problems,
- by loading in the Model Driven Service Abstraction Layer (MD-SAL) of the network controller, Services can be configured and chained together to match fluctuating needs,

Network programmability: OpenDayLight includes support OpenFlow and OpenFlow extensions such as Table Type Patterns (TTP), as well as traditional protocols including NETCONF, BGP/PCEP and CAPWAP. Additionally, OpenDayLight interfaces with [OpenStack](https://drive.google.com/file/d/0B_rLr6so6DZ8bHdtQkk0Rkk2Wms/view) and Open vSwitch.

Security: the platform provides a framework for Authentication, Authorization and Accounting (AAA), as well as automatic discovery and securing of network devices and controllers.

- [OpenDayLight Developer Guide](https://drive.google.com/file/d/0B_rLr6so6DZ8cXRJczlJSVBzOE0/view): corresponds to the Beryllium release of OpenDayLight, Feburary 2016

###  OPNFV

https://developer.cisco.com/site/opnfv/

## Private & Hybrid Cloud

### OpenStack contributions from CISCO

OpenDayLight, OPNFV see above

### Metapod   

- [Cisco Metapod](https://developer.cisco.com/site/Metapod/) : openstack pre-configured topology operated by Cisco on your premises

### Cloud infrastructure Management

- [Morpheus (Cisco partner)](https://www.morpheusdata.com/): Cloud Application Management and Orchestration Platform, infrastructure agnostic (On-premises Openstack, Cisco Metapod, Amazon AWS, Microsoft Azure)
