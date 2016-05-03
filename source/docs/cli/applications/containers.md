# Supergiant Component Container Control
## `supergiant <verb> component container`
*Prerequisite: You must have created a Spacetime Provider with `supergiant create spacetime provider`*
*Prerequisite: You must have created a Spacetime Kubernetes cluster with `supergiant create spacetime`*
*Prerequisite: You must have installed the Supergiant core with `supergiant create core`*
*Prerequisite: You must have created a Supergiant app with `supergiant create application`*
*Prerequisite: You must have created a Supergiant Component with `supergiant create component`*

The Container action allows the user to manage a container for a Component on their Supergiant cluster.

### Create component container:
#### `supergiant create component container <flags>`

Create component container will create a container inside a application component.

Help: `supergiant create component container --help`

Flags:

*Required*

`--comp <Component Name>` - The component the new container will be configured for.

`--app <Application Name>` - The Application where your component lives.

`--name <Volume Name>` - The name you would like to assign your container.

`--image <Docker Image>` - The docker image you would like to use with your container.

*Optional*

`--cpu-max <Max CPU Allocation>` - The maximum amount of CPU resource that will be allocated to your container. This number is expressed in Kubernetes resource [notation]().

`--cpu-min <Minimum CPU Allocation>` - The minimum amount of CPU resource that will be allocated to your container. This number is expressed in Kubernetes resource [notation]().

`--ram-max <Max RAM Allocation>` - The maximum amount of RAM to allocate for your container. This number is expressed in Kubernetes resource [notation]().

`--ram-min <Max RAM Allocation>` - The minimum amount of RAM to allocate for your container. This number is expressed in Kubernetes resource [notation]().

### Update component container:
#### `supergiant update component container <flags>`

Update component container will update a container inside a application component.

Help: `supergiant update component container --help`

Flags:

*Required*

`--comp <Component Name>` - The component the new container will be configured for.

`--app <Application Name>` - The Application where your component lives.

`--name <Volume Name>` - The name you would like to assign your container.

`--image <Docker Image>` - The docker image you would like to use with your container.

*Optional*

`--cpu-max <Max CPU Allocation>` - The maximum amount of CPU resource that will be allocated to your container. This number is expressed in Kubernetes resource [notation]().

`--cpu-min <Minimum CPU Allocation>` - The minimum amount of CPU resource that will be allocated to your container. This number is expressed in Kubernetes resource [notation]().

`--ram-max <Max RAM Allocation>` - The maximum amount of RAM to allocate for your container. This number is expressed in Kubernetes resource [notation]().

`--ram-min <Max RAM Allocation>` - The minimum amount of RAM to allocate for your container. This number is expressed in Kubernetes resource [notation]().

### Delete component container:
#### `supergiant delete component container <flags>`

Delete component container will delete a container inside a application component.

Help: `supergiant delete component container --help`

Flags:

*Required*

`--comp <Component Name>` - The component the new container will be configured for.

`--app <Application Name>` - The Application where your component lives.

`--name <Volume Name>` - The name you would like to assign your container.
