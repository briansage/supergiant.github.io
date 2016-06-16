[supergiant.io]: https://supergiant.io/ "Supergiant - Scaling Open-Source Container Orchestration"

# Glossary

## Application

An Application is a domain space for an organized group of Components that
should be designed to serve a purpose for your organization.

An example of an App might be _example.com_ or _Company Intranet_.


## Component

A Component runs a singular function, such as a database or search appliance. An
Application can be made up of many Components.


## Container

A Container holds a Docker image with RAM and CPU allocations, ports, and
environment variables. A Component requires at least one Container to run.


## Container Instances

A running Container. A Component may be configured to run multiple Container
Instances for application resiliency.


## Core

Core actions control the install and management of the Supergiant core
application on your Kubernetes cluster.


## Dashboard

The Supergiant GUI, accessible through a web browser.


## Deployments

...


## Docker

Docker containers allow software to be containerized into complete, runnable
filesystems, containing code, system tools, and linked libraries.

By making a Docker container, a lightweight app may be run anywhere, regardless
of the host system.


## Environment Variables

Container environment actions allows the user to manage container environment
variables for a component container.


## Kubernetes

From kubernetes.io: "Kubernetes is an open-source system for automating deployment, operations, and scaling of containerized applications. It groups containers that make up an application into logical units for easy management and discovery."


## Mount

A mount is the point that a volume is attached to a Container.


## Provider

The spacetime provider control tool allows the user to define cloud credentials
to use while performing supergiant actions. Spacetime maintains a separate
provider database in your spacetime config, because often a user may have or
want Kubernetes clusters to reside in multiple Regions, Zones, Accounts, or
Clouds using unique credentials.


## Packing Algorithm

The Packing Algorithm provisions the right resources when needed, lowering cost
and increasing hardware utilization, and ensuring you never have to worry about
managing servers directly.


## Port

A Container may be accessed via network ports, configured when you create a
Container with the Dashboard UI or when you create a release with the CLI.


## Releases

...


## Spacetime

Spacetime actions control Kubernetes clusters on which your supergiant core will
run. The spacetime controller on it's own is a useful way to manage multiple
Kubernetes clusters across multiple environments.


## Supergiant

[Supergiant][supergiant.io] is an open-source container orchestration system,
based on Kubernetes. It is built and maintained by the Qbox.io team to make it
easy to deploy stateful, distributed apps at scale.

Run dockerized apps and manage datacenter or cloud provisioned hardware like one
giant, self-healing computer. Supergiant's packing algorithm makes it easy to
reduce hardware expenses and gain performance.


## Supergiant API

The core of a Supergiant instance. The API exposes control of the general
provisioning of services and allocation of resources.



## Volume

A volume is persistent storage, like a solid state drive, IOPS drive, or
traditional disk drive. It is where data is stored.
