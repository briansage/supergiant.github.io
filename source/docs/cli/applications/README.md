# Supergiant Application Control

## `supergiant <verb> application`

| Prerequisites
| :---
| You must have created a Spacetime Provider with `supergiant create spacetime provider`
| You must have created a Spacetime Kubernetes cluster with `supergiant create spacetime`
| You must have installed the Supergiant core with `supergiant create core`

The Application action allows the user to create an application on their Supergiant cluster.

### Create application:

#### `supergiant create application <App Name> <flags>`

Create application will create a namespace in Kubernetes for your Spacetime components to live.

Help: `supergiant create application help`

Flags:

*optional*

`--kube <Kubernetes Cluster Name>` - The Kubernetes cluster where you would like to install the Supergiant core. This is optional, because you can use `supergiant select spacetime <Cluster name>` to select a current context for your Supergiant operations. When you `supergiant create spacetime import`, or `supergiant create spacetime` the resulting Kubernetes cluster is automatically selected as your current default cluster.

### Delete application:

#### `supergiant delete application <App Name> <flags>`

Delete application deletes an application from your spacetime cluster. All components contained in the application will also be destroyed.

Help: `supergiant delete application help`

Flags:

*optional*

`--kube <Kubernetes Cluster Name>` - The Kubernetes cluster where you would like to install the Supergiant core. This is optional, because you can use `supergiant select spacetime <Cluster name>` to select a current context for your Supergiant operations. When you `supergiant create spacetime import`, or `supergiant create spacetime` the resulting Kubernetes cluster is automatically selected as your current default cluster.
