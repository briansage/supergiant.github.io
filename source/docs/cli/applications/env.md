# Supergiant Component Container Environment Control
## `supergiant <verb> component env`
*Prerequisite: You must have created a Spacetime Provider with `supergiant create spacetime provider`*

*Prerequisite: You must have created a Spacetime Kubernetes cluster with `supergiant create spacetime`*

*Prerequisite: You must have installed the Supergiant core with `supergiant create core`*

*Prerequisite: You must have created a Supergiant app with `supergiant create application`*

*Prerequisite: You must have created a Supergiant Component with `supergiant create component`*

*Prerequisite: You must have created a Supergiant Component container with `supergiant create component container`*

The Container environment action allows the user to manage container environment variables for a component container.

### Create component container environment command:
#### `supergiant create component env <flags>`

Create component container command will add a new environment variable to your component container.

Help: `supergiant create component env --help`

Flags:

*Required*

`--comp <Component Name>` - The component the new container will be configured for.

`--app <Application Name>` - The Application where your component lives.

`--name <Volume Name>` - The name of the container where the command will get assigned.

`--var <Variable Name>` - The name of the environment variable to use.

`--value <Variable Value>` - The value for your environment variable.

### Update component container environment:
#### `supergiant update component env <flags>`

Update component container environment updates an existing container environment variable with a new value.

Help: `supergiant update component env --help`

Flags:

*Required*

`--comp <Component Name>` - The component the new container will be configured for.

`--app <Application Name>` - The Application where your component lives.

`--name <Volume Name>` - The name of the container where the command will get assigned.

`--var <Variable Name>` - The name of the environment variable to use.

`--value <Variable Value>` - The value for your environment variable.



### Delete component container environment:
#### `supergiant delete component env <flags>`

Delete component container environment will delete a environment variable in a component container.

Help: `supergiant delete component env --help`

Flags:

*Required*

`--comp <Component Name>` - The component the new container will be configured for.

`--app <Application Name>` - The Application where your component lives.

`--name <Volume Name>` - The name of the container where the command will get assigned.

`--var <Variable Name` - The name of the environment variable to use.
