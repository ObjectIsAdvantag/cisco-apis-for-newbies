# About

This guide is a tentative to synthesize Cisco APIs for developers & ITPros with no to little knowledge of Cisco lines of hardware and software products.
Started as a tribute to my "First Days Party" @Cisco Live Berlin Feb15-19 2016.
Contributors welcome, CC BY 4.0 licence.


# New to Cisco for developers ?

You definitely need to check the [DevNet portal](https://developer.cisco.com/site/devnet/home/index.gsp), the one-stop for all development related activites with/to/from/above CISCO technologies.

Take a few minutes to create your accout, it's really worth it :
- [DevNet](https://developer.cisco.com/site/devnet/home/index.gsp): umbrella to technical resources about IoT, Cloud, Networking, Data Center, Collaboration, Analytics & Automation, Security, Services, DevOps, Microservices
- [Learning labs](https://learninglabs.cisco.com/springboards) : step by step walkthroughs for developers, featuring live environments / sandboxes to interact with CISCO Hardware via REST APIs
- [Programming foundation](https://learninglabs.cisco.com/modules/programming-found) : learn REST principles and how to call them via a User Interface, from the command line, or from code
- [Sandbox](https://developer.cisco.com/site/devnet/sandbox/): provision various CISCO hardware and network topologies and experiment Live APIs. Environments are provisionned for your own use from 3 hours to 7 days. APIC-EM , Cisco Open SDN Controller , Jabber , Webex , Intercloud Fabric...
- [DevNet Labs](https://developer.cisco.com/site/devnetlabs/) : Showcase of software projects built out of CISCO APIs and open technologies contributed by Cisco


# Collaboration APIs

## Tropo

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


## Cisco Spark

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


## WebEx

- [WebEx APIs](https://developer.cisco.com/site/webex-developer/develop-test/try-webex-apis/)
- [DevNet Sandbox](https://developer.cisco.com/site/devnet/sandbox/available-labs/comm-collab/) : explore Cisco WebEx API capabilities and start developing your proof-of-concept solution
- [WebEx Developer Program](https://developer.cisco.com/site/webex-developer/web-conferencing/program-benefits/)


# Hardware and Network capable APIs

[All about Cisco networking technologies for developers](https://developer.cisco.com/networking)


## SDN - Software Defined Network APIs

### ACI/APIC

### OpenDayLight

[OpenDaylight](https://www.opendaylight.org/platform-overview-beryllium), the open SDN platform, aims to make interoperable, programmable networks a reality.

Why OpenDaylight ? with SDN, you can achieve network programmability and abstraction, but then comes the question of managing it.
Via common API frameworks, OpenDayLight helps create abstractions North or South of the controller without having to look under the hood. Approaches to intent and policy to do this: ALTO, Group Based Policy and Network Intent Composition.

OpenDayLight delivers the benefits of both Software Defined Networks (SDN) and Network Functions Virtualization (NFV).

[Major use cases](https://www.opendaylight.org/use-cases/) include Automated / Agile / OnDemand Service Delivery and Dynamic Network Resources Optimization.


## Configure your network

- [RESTCONF](http://sdntutorials.com/what-is-restconf)
- [Cisco Prime Infrastructure API](https://developer.cisco.com/site/prime-infrastructure/documents/api-reference/api-reference/)

## Private cloud

### Metapod   

- [Cisco Metapod](https://developer.cisco.com/site/Metapod/) : openstack pre-configured topology operated by Cisco on your premises

## Hybrid cloud

- [Morpheus (Cisco partner)](https://www.morpheusdata.com/): Cloud Application Management and Orchestration Platform, infrastructure agnostic

# Data

## Cisco Zeus (Cloud offering, Restricted Beta)

Zeus is a Cloud-based Logging and Monitoring Service. Use the Zeus API or standard agents (such as fluent, syslog, logstash, collectd, statsd) to push your logs and metrics to Zeus.
Interactively visualize, search or analyze your data, or query / aggregate via the Zeus API.

- [Zeus Portal](http://www.ciscozeus.io/) : request access to the beta
- [Github Repo](https://github.com/CiscoZeus) : python , ruby, java and go clients
- [API Documentation](http://api.ciscozeus.io/) : Swagger UI
- [Getting started guide](http://blogs.ciscozeus.io/2015/09/getting-started-with-logs-and-metrics.html)
- [Zeus Blog](http://blogs.ciscozeus.io/


# Other cool Cisco technologies for developers

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

- [NeXt](https://developer.cisco.com/site/neXt/)
