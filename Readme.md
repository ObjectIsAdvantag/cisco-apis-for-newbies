# Everything API-enabled at Cisco

This guide is an opinionated tentative to synthesize [Cisco APIs for developers & network engineers](https://developer.cisco.com/site/devnet/index/) with no to little knowledge of Cisco hardware, software and solutions.
Started as a tribute to my "First Days Party" at Cisco Live Berlin Feb 15-19th 2016.
Contributors welcome, CC BY 4.0 license.

- [New to Cisco APIs](#toc_DevNet)
- [Collaboration](#toc_Collaboration)
- [Data & Analytics](#toc_Data)
- [DevOps, Software Tools & Automation](#toc_DevOps)
- [IoT](#toc_IoT)
- [Private & Hybrid Cloud](#toc_PrivateCloud)
- [Programmable networks](#toc_Networking)


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
- [Twitter @Tropo](https://twitter.com/Tropo)
   - [@TropoChanges](https://twitter.com/tropochanges) : get realtime insights to Tropo Cloud
   - evangelists: [adam](https://twitter.com/akalsey), [diggz](https://twitter.com/JohnnyDiggz), [marcello](https://twitter.com/marchfederico), [paul](https://twitter.com/paultodwyer), [phil](https://twitter.com/PBellanti), [steve](https://twitter.com/ObjectIsAdvantag)


## <a name="toc_Spark"></a>Cisco Spark

Since March 2015, [Cisco Spark](https://www.ciscospark.com/) is the all-in-one Cloud Collaboration platform for the extended enterprise.
In short, Cisco Spark is a multi-client platform (Phone, Mac, Windows apps), backed by Cloud Collaboration Services (persistent chat rooms, WebRTC video conferencing), enabling 1-1, 1-few, 1-many communication.
Cisco Spark can be used for short-live meeting rooms, but also long-live collaborative workspaces, opened to internal co-workers, but also partners and external communities.

The overall Cisco Spark platform can be managed via [REST APIs](https://developer.ciscospark.com/getting-started.html) : easily bring messaging capabilities into your apps, automatically send messages to Spark rooms based on real-world/business events.

- [Spark APIs](https://developer.ciscospark.com/getting-started.html): REST APIs interactive documentation
- [Spark for developers](https://developer.cisco.com/site/spark/): the DevNet umbrella for all Spark related contents for developers
- [Learning labs](https://developer.cisco.com/site/spark/): Rooms and messages, Authentication, WebHooks
- [Twitter @CiscoSparkDev](https://twitter.com/ciscosparkdev)
   - evangelists: [adam](https://twitter.com/akalsey), [diggz](https://twitter.com/JohnnyDiggz), [marcello](https://twitter.com/marchfederico), [paul](https://twitter.com/paultodwyer), [phil](https://twitter.com/PBellanti), [steve](https://twitter.com/ObjectIsAdvantag)
   - consulting: [Fabien Medat](https://www.ciscospark.com/): head of technical consulting for Collaboration French Team

## <a name="toc_WebEx"></a>WebEx

- [WebEx APIs](https://developer.cisco.Fcom/site/webex-developer/develop-test/try-webex-apis/)
- [DevNet Sandbox](https://developer.cisco.com/site/devnet/sandbox/available-labs/comm-collab/) : explore Cisco WebEx API capabilities and start developing your proof-of-concept solution
- [WebEx Developer Program](https://developer.cisco.com/site/webex-developer/web-conferencing/program-benefits/)

## <a name="toc_InstantConnect"></a>Cisco Instant Connect

Instant Connect is a push-to-talk (PTT) communication product for Android devices & Cisco Wireless IP Phones: create instant group and private audio connectivity and collaboration, while saving money compared to carrier-based PTT services.

- [DevNet Central](https://developer.cisco.com/site/cisco-instant-connect/)
- [API documentation](http://www.cisco.com/c/en/us/td/docs/interoperability_systems/c_ipics/461/api/guide/api461/restfunc.html) : WebServices and REST API Cisco IP Interoperability and Collaboration System (IPICS) release 4.6(x) application programming interface
(API)

# <a name="toc_Data"></a>Data & Analytics

Digitalization & IoT are challenging enterprises to seek new ways to manage and leverage their data: store, gather, analyse, act.

- [Cisco Data and Analytics solutions](http://www.cisco.com/c/en/us/products/analytics-automation-software/data-analytics-software/index.html#~tab-products)
- [Twitter @CiscoAnalytics](https://twitter.com/CiscoAnalytics)

## Distributed Network analytics

Orchestrate the generation and collection of telemetry data inside a network, and process streaming analytics. Strategy here is to bring the analytics processing of close as possible to the Data.

The platform is model-driven, open and modular, and comes with 2 components.
On top of a network controller (APIC-EM or OpenDayLight), the Analytics controller expands a YANG-based Analytics model, deploys the configuration to the agents, then collects data and correlates among agents.
Analytics Agents reside on the devices, as linux containerized apps, collect data and embedd the Connected Streaming Analytics (CSA) software to ensure local data processing.

- [Documentation](http://www.cisco.com/c/en/us/td/docs/net_mgmt/prime/analytics/1-1-1/quick_start/guide/ConnectedStreamingAnalytics-1-1-1-QuickStartGuide.pdf)


## PaNDA (to be opensourced in March 2016)

PaNDA is a simple, scalable and open platform for networks analytics, including operational intelligence (OSS) and business intelligence applications (BSS), designed to scale up to consume millions of messages per second.

The platform is based on open source technologies centered on Apache Hadoop and Kafka, main processing workhorses are Apache Spark and Spark Streaming. Ingested data should be encapsulated in an Avro schema and published on a pre-defined Kafka topics.

- [Cisco PaNDA](http://panda.cisco.com/)
- [DevNet Portal](https://developer.cisco.com/site/panda/)
- [Data preparation](http://panda.cisco.com/documentation/20-datapreparation)
- UseCases : Network Service Assurance, IoT
- [DevNet Learning lab](https://learninglabs.cisco.com/labs/tags/PaNDA)


## Cisco Zeus (Cloud offering, Restricted Beta)

Zeus is a Cloud-based Logging and Monitoring Service. Use the Zeus API or standard agents (such as fluent, syslog, logstash, collectd, statsd) to push your logs and metrics to Zeus.
Interactively visualize, search or analyze your data, or query / aggregate via the Zeus API.

- [Zeus Portal](http://www.ciscozeus.io/) : request access to the beta
- [Github Repo](https://github.com/CiscoZeus) : python , ruby, java and go clients
- [API Documentation](http://api.ciscozeus.io/) : Swagger UI
- [Getting started guide](http://blogs.ciscozeus.io/2015/09/getting-started-with-logs-and-metrics.html)
- [Zeus Blog](http://blogs.ciscozeus.io/


# <a name="toc_DevOps"></a>DevOps, Software Tools & Automation

## Operating Systems

Cisco 's Networking operating systems, operating on millions of active systems, ranging from the small home office router to the core systems of the world's largest service provider networks.

### Cisco IOS (closed source, current release: 15)

- [Product Portal](http://www.cisco.com/c/en/us/products/ios-nx-os-software/ios-software-releases-listing.html)
- [IOS capabilities](http://www.cisco.com/c/en/us/products/ios-nx-os-software/ios-technologies/index.html): IPv6, IP Multicast, IP Routing, IP Mobility, Instrumentation, MPLS, Security, High Availability, QoS, VPN

### Cisco IOS-XR (closed source, current release: 5.1)

- [Product Portal](http://www.cisco.com/c/en/us/products/ios-nx-os-software/ios-xr-software/index.html); Modular and fully distributed network operating system  for service providers
- [Realtime Monitoring @DevNet](https://developer.cisco.com/site/ios-xr/)

### Cisco IOS-XE (closed source, current release: 3)

- [Product Portal](http://www.cisco.com/c/en/us/products/ios-nx-os-software/ios-xe/index.html): Supports next-generation platforms, Runs as a single daemon within a modern Linux operating system

### Cisco IOx

IOx brings together Cisco IOS and Linux, giving the opportunity to deploy Linux applications on edge IOS network devices. Use cases: create IoT applications such as data aggregation, control systems, access control and have them run on the edge.

- [DevNet Central](https://developer.cisco.com/site/iox/technical-overview/)

### Cisco NX-OS

Network operating system for the Nexus-series and MDS-series Ethernet switches.

- [Product Portal](http://www.cisco.com/c/en/us/products/ios-nx-os-software/nx-os/index.html)
- [Open NX-OS](https://opennxos.cisco.com/public/learn): software suite that exposes APIs, data models, and programmatic constructs, introduced from NX-OS release 7.


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


# <a name="toc_IoT"></a>IoT

- [DevNet IoT Central](https://developer.cisco.com/site/internet-of-things/)

## CMX Mobility Services (Released)

Triangulate device location using wifi, and track location via device's mac address.

- [DevNet CMX Mobility Services]()
- Use Cases: coupons, promotions, push notifications

## <a name="toc_DMO"></a>Data in Motion (Released)

Over the next 7-10 years the number of smart objects will grow to be over 50 billion. To overcome the expected deluge of data, Data in Motion (DMo) is a piece of software that provides data management and first-order analysis at the edge (ie, on the network components the IoT devices are attached to). By distributing and optimizing the processing and storage of data on the edge, DMO ensure yours apps can manage flows of Data at scale.

As of March 2016, Data in Motion is supported on Cisco UCS C-series and E-series

- [DevNet Data In Motion Central](https://developer.cisco.com/site/data-in-motion/)
- [Big Picture](https://developer.cisco.com/site/data-in-motion/discover/overview/)
- [REST API](https://developer.cisco.com/site/data-in-motion/documents/api-reference/index.gsp#restful-api) : restful-api with WebDAV extensions to manage
- [Reference guide](https://developer.cisco.com/fileMedia/download/d3b70460-0f0a-4ff6-954a-7066bc4982c0)
- Uses cases:
   - Energy Utility Companies Process: 1.1 BILLION Data Points (.5TB) per Day
   - A Large Offshore Field Produces: 0.75TB of Data Weekly
   - An Airplane: 10TB of Data for Every 30 Minutes of Flight

## Jasper (Acquisition announced Feb 2016)

The Jasper IoT service platform - Control Center - automates your IoT services across connected devices : launch, manage, and monetize IoT services, over more than 100 countries thanks to Jasper production-ready partnerships with more than 25 Mobile operators.

- [Jasper Corporate Portal](http://www.jasper.com/)
- [Acquisition](http://newsroom.cisco.com/press-release-content?articleId=1741680)
- [Twitter](https://twitter.com/Jasper_IoT)


# <a name="toc_PrivateCloud"></a>Private & Hybrid Cloud

## Metapod

Cisco Metapod is a production-ready private cloud infrastructure based on [OpenStack](#toc_OpenStack).
Metapod  is custom-engineered, deployed, and remotely operated 24x7x365 by Cisco.
Cisco provides platform and security updates, operates the platform with 99.99% SLA guarantees and supports enterprise capacity planning requirements.

- [Cisco Metapod](http://www.cisco.com/c/en/us/products/cloud-systems-management/metapod/index.html)
- [DevNet Metapod Center](https://developer.cisco.com/site/Metapod/)
- [API compatibility](http://www.cisco.com/c/en/us/products/cloud-systems-management/metapod/api-compatibility.html): 100% API coverage for computing and storage, OpenStack APIs, AWS compatible APIs for core services, Native API support to automation and tooling platforms (Chef, Puppet, Salt, Ansible, Fog, libcloud, jclouds...) and many more)

### <a name="toc_OpenStack"></a>OpenStack contributions

OpenStack is a large open source software project that provides a platform for creating, operating, and consuming public and private clouds. OpenStack abstracts key elements of a datacenter - compute, storage, and networking resources, into pools of resource accessible by a unified API. As a OpenStack cloud tenant or a cloud application, you can use these APIs to provision these resources within the limits set by the administrator.

- [OpenStack at Cisco](https://developer.cisco.com/site/openstack/discover/overview/): Cisco’s technical and operational involvement with OpenStack
   - [Cisco products integration](https://developer.cisco.com/site/openstack/downloads/openstack-integration/)
- [OpenStack on your laptop](https://learninglabs.cisco.com/labs): self-paced lab to install and start using OpenStack within a virtual machine (VM)

## Hybrid cloud

### CliQr

CliQr CloudCenter is a platform to model, deploy and manage the entire lifecycle of applications onto 15 public (Amazon Web Services, Google Compute Platform, Microsoft Azure, Rackspace, IBM, NTT...) and private cloud environments (VMWare, OpenStack, Cisco UCS director...)

- [Cliqr](http://www.cliqr.com/platform/)
- [CloudCenter API](http://docs.cliqr.com/display/40API/CloudCenter+API+Overview)
- [Acquisition announcement](http://newsroom.cisco.com/press-release-content?type=webcontent&articleId=1750092)
- [Twitter](https://twitter.com/CliQrTech)


### Partners

- [Morpheus (Cisco partner)](https://www.morpheusdata.com/): Cloud Application Management and Orchestration Platform, infrastructure agnostic (On-premises Openstack, Cisco Metapod, Amazon AWS, Microsoft Azure)

## Cloud native platform

### CloudFoundry

The [CloudFoundry PaaS](http://pivotal.io/cisco) - installed onto [Cisco Metapod](#toc_Metapod) private cloud infrastructure - enables enterprises to rapidly deploy new applications using any language/runtime and leveraging various backing services.

- [Peder Ulander](pulander@cisco.com): Cisco’s VP of Cloud and Managed Services


# <a name="toc_Networking"></a>Programmable networks

Since March 2016, the umbrella terminology is [Cisco DNA (Digital Network Architecture)]().

- [DevNet Networking Portal](https://developer.cisco.com/networking): all about Cisco network programming for developers network engineers

## Configure your network

- [RESTCONF](http://sdntutorials.com/what-is-restconf) : HTTP-based protocol, which provides REST-like APIs to manipulate YANG modeled data and invoke YANG modeled RPCs, using XML or JSON as payload format

- [NETCONF]() : XML-based RPC protocol, which provides abilities for client to invoke YANG-
modeled RPCs, receive notifications and to read, modify and manipulate YANG modeled data.

- [Cisco Prime Infrastructure API](https://developer.cisco.com/site/prime-infrastructure/documents/api-reference/api-reference/)

## Software Defined Network (SDN) & Network Functions Virtualization (NFV)

### ACI/APIC

### OpenDayLight

[OpenDaylight](https://www.opendaylight.org/) aims to make interoperable and programmable networks a reality, by delivering the benefits of Software Defined Networks (SDN) and Network Functions Virtualization (NFV) to networks of any size and scale. [Use cases](https://www.opendaylight.org/use-cases/) include Automated / Agile / OnDemand Service Delivery and Dynamic Network Resources Optimization.

[How ?](https://www.opendaylight.org/platform-overview-beryllium) with SDN, you can achieve network programmability and abstraction, but then comes the question of managing it. Via common API frameworks, OpenDayLight helps create abstractions North or South of the controller without having to look under the hood. Several  intent and policy approaches to do this include ALTO, Group Based Policy and Network Intent Composition.

Architecture: OpenDayLight employs a model-driven approach to describe the network, the functions to be performed on it and the resulting state or status achieved.
- by sharing YANG data structures in a common data store and messaging infrastructure, OpenDaylight allows for fine-grained services to be created then combined together to solve more complex problems,
- by loading in the Model Driven Service Abstraction Layer (MD-SAL) of the network controller, Services can be configured and chained together to match fluctuating needs,

Network programmability: OpenDayLight includes support OpenFlow and OpenFlow extensions such as Table Type Patterns (TTP), as well as traditional protocols including NETCONF, BGP/PCEP and CAPWAP. Additionally, OpenDayLight interfaces with [OpenStack](https://drive.google.com/file/d/0B_rLr6so6DZ8bHdtQkk0Rkk2Wms/view) and Open vSwitch.

Security: the platform provides a framework for Authentication, Authorization and Accounting (AAA), as well as automatic discovery and securing of network devices and controllers.

- [OpenDayLight Developer Guide](https://drive.google.com/file/d/0B_rLr6so6DZ8cXRJczlJSVBzOE0/view): corresponds to the Beryllium release of OpenDayLight, Feburary 2016
- [Twitter](https://twitter.com/OpenDaylightSDN)


###  OPNFV

https://developer.cisco.com/site/opnfv/
