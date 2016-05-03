# Supergiant Component Container Port Control
## `supergiant <verb> component port`
*Prerequisite: You must have created a Spacetime Provider with `supergiant create spacetime provider`*

*Prerequisite: You must have created a Spacetime Kubernetes cluster with `supergiant create spacetime`*

*Prerequisite: You must have installed the Supergiant core with `supergiant create core`*

*Prerequisite: You must have created a Supergiant app with `supergiant create application`*

*Prerequisite: You must have created a Supergiant Component with `supergiant create component`*

*Prerequisite: You must have created a Supergiant Component container with `supergiant create component container`*

The container port action allows the user to manage container ports for a component container.

### Create component container port command:
#### `supergiant create component port <flags>`

Create component container port will add a new port to your component container.

Help: `supergiant create component port --help`

Flags:

*Required*

`--comp <Component Name>` - The component the new container will be configured for.

`--app <Application Name>` - The Application where your component lives.

`--name <Container Name>` - The name of the container where the command will get assigned.

`--protocol <Protocol>` - The protocol to use with the port. i.e. "http" or "tcp"

`--port-number <Port Number>` - The port number to use.

*Optional*

`--public` - A bool flag telling Supergiant that this port should be public accessible from outside your Supergiant cluster.

`--entrypoint <Entry Point Name>` - The name of the [entry point]() to use for your port.

`--external-port-number <Port Number>` - The external facing port number of your public port. NOTE: If you use this feature, you must manage your ports as to not conflict with any other manually set external ports. By default Supergiant will use the randomly generated external port provided by Kubernetes as your external port number.  


### Update component container port:
#### `supergiant update component port <flags>`

Update component container port updates an existing container port with a new configuration.

Help: `supergiant update component port --help`

Flags:

*Required*

`--comp <Component Name>` - The component the new container will be configured for.

`--app <Application Name>` - The Application where your component lives.

`--name <Container Name>` - The name of the container where the command will get assigned.

`--protocol <Protocol>` - The protocol to use with the port. i.e. "http" or "tcp"

`--port-number <Port Number>` - The port number to use.

*Optional*

`--public` - A bool flag telling Supergiant that this port should be public accessible from outside your Supergiant cluster.

`--entrypoint <Entry Point Name>` - The name of the [entry point]() to use for your port.

`--external-port-number <Port Number>` - The external facing port number of your public port. NOTE: If you use this feature, you must manage your ports as to not conflict with any other manually set external ports. By default Supergiant will use the randomly generated external port provided by Kubernetes as your external port number.  



### Delete component container port:
#### `supergiant delete component port <flags>`

Delete component container port will delete a port in a component container.

Help: `supergiant delete component port --help`

Flags:

*Required*

`--comp <Component Name>` - The component the new container will be configured for.

`--app <Application Name>` - The Application where your component lives.

`--name <Container Name>` - The name of the container where the command will get assigned.

`--port-number <Port Number>` - The internal port number of the port you would like to delete. 
