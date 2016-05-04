# Supergiant Core Control
## `supergiant <verb> core`

| Prerequisites
| :---
| You must have created a Spacetime Provider with `supergiant create spacetime provider`
| You must have created a Spacetime Kubernetes cluster with `supergiant create spacetime`

Core actions control the install and management of the Supergiant core application on your Kubernetes cluster.

### Create core:
#### `supergiant create core <flags>`

Create core will install the latest available supported version of the supergiant core to your cluster.

Help: `supergiant create core help`

Flags:

*optional*

`--kube <Kubernetes Cluster Name>` - The Kubernetes cluster where you would like to install the Supergiant core. This is optional, because you can use `supergiant select spacetime <Cluster name>` to select a current context for your Supergiant operations. When you `supergiant create spacetime import`, or `supergiant create spacetime` the resulting Kubernetes cluster is automatically selected as your current default cluster.

### Update core:
#### `supergiant update core <flags>`

Update core will rebuild your supergiant installation without touching the it's database. This can be useful for updating to newer versions of the core.

Help: `supergiant update core help`

Flags:

*optional*

`--kube <Kubernetes Cluster Name>` - The Kubernetes cluster where you would like to install the Supergiant core. This is optional, because you can use `supergiant select spacetime <Cluster name>` to select a current context for your Supergiant operations. When you `supergiant create spacetime import`, or `supergiant create spacetime` the resulting Kubernetes cluster is automatically selected as your current default cluster.

`--version <version>` - This option allows you to select any version available on the Supergiant api public [docker-hub page](https://hub.docker.com/r/supergiant/supergiant-api/tags/). By default the CLI will choose it known latest stable version.

### Delete core:
#### `supergiant delete core <flags>`

Why would you want to do that?

Help: `supergiant delete core help`

Flags:

*optional*

`--kube <Kubernetes Cluster Name>` - The Kubernetes cluster where you would like to install the Supergiant core. This is optional, because you can use `supergiant select spacetime <Cluster name>` to select a current context for your Supergiant operations. When you `supergiant create spacetime import`, or `supergiant create spacetime` the resulting Kubernetes cluster is automatically selected as your current default cluster.
