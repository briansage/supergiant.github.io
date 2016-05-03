# Supergiant Component Container Mount Control
## `supergiant <verb> component mount`
*Prerequisite: You must have created a Spacetime Provider with `supergiant create spacetime provider`*

*Prerequisite: You must have created a Spacetime Kubernetes cluster with `supergiant create spacetime`*

*Prerequisite: You must have installed the Supergiant core with `supergiant create core`*

*Prerequisite: You must have created a Supergiant app with `supergiant create application`*

*Prerequisite: You must have created a Supergiant Component with `supergiant create component`*

*Prerequisite: You must have created a Supergiant Component container with `supergiant create component container`*

The container mount action allows the user to manage container mounts for a component container.

### Create component container mount command:
#### `supergiant create component mount <flags>`

Create component container mount will add a new mount to your component container.

Help: `supergiant create component mount --help`

Flags:

*Required*

`--comp <Component Name>` - The component the new container will be configured for.

`--app <Application Name>` - The Application where your component lives.

`--name <Volume Name>` - The name of the container where the command will get assigned.

`--path <Mount Path>` - The path where a volume will be mounted inside your container.

`--volume <Volume Name>` - The name of the volume to be used with this mount point.

### Update component container mount:
#### `supergiant update component mount <flags>`

Update component container mount updates an existing container mount with a new configuration.

Help: `supergiant update component mount --help`

Flags:

*Required*

`--comp <Component Name>` - The component the new container will be configured for.

`--app <Application Name>` - The Application where your component lives.

`--name <Volume Name>` - The name of the container where the command will get assigned.

`--path <Mount Path>` - The path where a volume will be mounted inside your container.

`--volume <Volume Name>` - The name of the volume to be used with this mount point.



### Delete component container mount:
#### `supergiant delete component mount <flags>`

Delete component container mount will delete a mount point in a component container.

Help: `supergiant delete component mount --help`

Flags:

*Required*

`--comp <Component Name>` - The component the new container will be configured for.

`--app <Application Name>` - The Application where your component lives.

`--name <Container Name>` - The name of the container where the command will get assigned.

`--path <Mount Path>` - The path where a volume will be mounted inside your container.
