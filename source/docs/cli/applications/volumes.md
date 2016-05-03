# Supergiant Component Volume Control
## `supergiant <verb> component volume`
*Prerequisite: You must have created a Spacetime Provider with `supergiant create spacetime provider`*
*Prerequisite: You must have created a Spacetime Kubernetes cluster with `supergiant create spacetime`*
*Prerequisite: You must have installed the Supergiant core with `supergiant create core`*
*Prerequisite: You must have created a Supergiant app with `supergiant create application`*
*Prerequisite: You must have created a Supergiant Component with `supergiant create component`*

The Volume action allows the user to manage a volume for a Component on their Supergiant cluster.

### Create component volume:
#### `supergiant create component volume <flags>`

Create component volume will create a volume in your Supergiant component that containers can then mount as persistent volume stores. The Supergiant core will ensure multiple instances of your component are provided with a unique version of the volume for every instance. Component volumes can be thought of as a "blueprint" for each instance of your component to use when creating persistent storage.

Help: `supergiant create component volume --help`

Flags:

*Required*

`--comp <Component Name>` - The component the new volume will be configured for.

`--app <Application Name>` - The Application where your component lives.

`--name <Volume Name>` - The name you would like to assign your volume. This name is used in the mount section of the container to reference the volume.

*Optional*

`--type <Storage Type>` - The type of storage you would like to use. Defaults to "gp2" (SSD), other options: "io1" (Provisioned IOPS), "magnetic" (Traditional Rotating Magnetic Drives)

`--size <size>` - The size you would like the drive to be in GB. Defaults to 20, but can be set from 1 to 16384.

### Update component volume:
#### `supergiant update component volume <flags>`

Update component volume allows the user to update the type, or size of their volume. Supergiant will automatically make the requested modification, snapshot, and migrate your volume. Components using the volume will then restart and use the updated configuration. This feature is especially useful when the user needs to increase the size of a volume that is reaching the limit of it's capacity.

Flags:

*Required*

`--comp <Component Name>` - The component the new volume will be configured for.

`--app <Application Name>` - The Application where your component lives.

`--name <Volume Name>` - The name you would like to assign your volume. This name is used in the mount section of the container to reference the volume.

*Optional*

`--type <Storage Type>` - The type of storage you would like to use. Defaults to "gp2" (SSD), other options: "io1" (Provisioned IOPS), "magnetic" (Traditional Rotating Magnetic Drives)

`--size <size>` - The size you would like the drive to be in GB. Defaults to 20, but can be set from 1 to 16384.

### Delete component volume:
#### `supergiant delete component volume <flags>`

Delete component volume deletes a volume configuration from a application component.

Flags:

*Required*

`--comp <Component Name>` - The component the new volume will be configured for.

`--app <Application Name>` - The Application where your component lives.

`--name <Volume Name>` - The name you would like to assign your volume. This name is used in the mount section of the container to reference the volume.
