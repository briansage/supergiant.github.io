# Glossary

## Application

An Application is a domain space for an organized group of Components that
should be designed to serve a purpose for your organization.

An example of an App might be _example.com_ or _Company Intranet_.


## Component

A Component runs a singular function, such as a database or search appliance. An
Application can be made up of many Components.


## Container Instances

...


## Container

A Container holds a Docker image with RAM and CPU allocations, ports, and
environment variables. A Component requires at least one Container to run.


## Core

Core actions control the install and management of the Supergiant core
application on your Kubernetes cluster.


## Dashboard

...


## Deployments

...


## Docker

...

## Environment Variables

Container environment actions allows the user to manage container environment
variables for a component container.


## Kubernetes

...

## Mount

A mount is the point that a volume is attached to a Container.


## Provider

The spacetime provider control tool allows the user to define cloud credentials
to use while performing supergiant actions. Spacetime maintains a separate
provider database in your spacetime config, because often a user may have or
want Kubernetes clusters to reside in multiple Regions, Zones, Accounts, or
Clouds using unique credentials.


## Packing Algorithm

...

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

The first datacenter total control system that makes it easy to manage stateful,
distributed apps. With Supergiant, you can run dockerized apps and manage
hardware like one giant, efficient computer. Supergiant makes it easy to deploy
faster and reduce hardware expenses.


## Supergiant API

...


## Volume

A volume is persistent storage, like a solid state drive, IOPS drive, or
traditional disk drive. It is where data is stored.
