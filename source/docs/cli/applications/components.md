# Supergiant Component Control

## `supergiant <verb> component`

| Prerequisites
| :---
| You must have created a Spacetime Provider with `supergiant create spacetime provider`
| You must have created a Spacetime Kubernetes cluster with `supergiant create spacetime`
| You must have installed the Supergiant core with `supergiant create core`
| You must have created a Supergiant app with `supergiant create application`

The Component action allows the user to create a component for an application on their Supergiant cluster.

### Create component:
#### `supergiant create component <Comp Name> <flags>`

Create component will create a namespace in Kubernetes for your containerized applications to live.

Help: `supergiant create component help`

Flags:

*optional*

`--kube <Kubernetes Cluster Name>` - The Kubernetes cluster where you would like to install the Supergiant core. This is optional, because you can use `supergiant select spacetime <Cluster name>` to select a current context for your Supergiant operations. When you `supergiant create spacetime import`, or `supergiant create spacetime` the resulting Kubernetes cluster is automatically selected as your current default cluster.

### Delete component:
#### `supergiant delete component <Comp Name> <flags>`

Delete component deletes an component from a Spacetime application.

Help: `supergiant delete application help`

Flags:

*optional*

`--kube <Kubernetes Cluster Name>` - The Kubernetes cluster where you would like to install the Supergiant core. This is optional, because you can use `supergiant select spacetime <Cluster name>` to select a current context for your Supergiant operations. When you `supergiant create spacetime import`, or `supergiant create spacetime` the resulting Kubernetes cluster is automatically selected as your current default cluster.
