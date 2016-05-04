# Supergiant Component Container Command Control

## `supergiant <verb> component command`

| Prerequisites
| :---
| You must have created a Spacetime Provider with `supergiant create spacetime provider`
| You must have created a Spacetime Kubernetes cluster with `supergiant create spacetime`
| You must have installed the Supergiant core with `supergiant create core`
| You must have created a Supergiant app with `supergiant create application`
| You must have created a Supergiant Component with `supergiant create component`
| You must have created a Supergiant Component container with `supergiant create component container`

The Container action allows the user to manage a container for a Component on their Supergiant cluster.

### Create component container command:
#### `supergiant create component command <flags>`

Create component container command will add a new command string to a component container.

Help: `supergiant create component container --help`

Flags:

*Required*

`--comp <Component Name>` - The component the new container will be configured for.

`--app <Application Name>` - The Application where your component lives.

`--name <Volume Name>` - The name of the container where the command will get assigned.

`--cmd <Command> --cmd <Command>...` - A argument list of commands to assign to your container. Usage here is a little weird, but each `--cmd` flag corresponds to a field or argument in your container. For Example:

If my application container required these command line options: `/my-app --foo bar --nuts bolts` the corresponding supergiant command would look like this:
`supergiant create component command --app <your app name> --comp <your component name> --name <your container name> --cmd "/my-app" --cmd "--foo" --cmd "bar" --cmd "--nuts" --cmd "bolts"`


### Delete component container commands:
#### `supergiant delete component command <flags>`

Delete component container commands will delete a command in a component container.

Help: `supergiant delete component command --help`

Flags:

*Required*

`--comp <Component Name>` - The component the new container will be configured for.

`--app <Application Name>` - The Application where your component lives.

`--name <Volume Name>` - The name of the container where the command will get assigned.

`--cmd <Command> --cmd <Command>...` - A argument list of commands to assign to your container. Usage here is a little weird, but each `--cmd` flag corresponds to a field or argument in your container. For Example:

If my application container required these command line options: `/my-app --foo bar --nuts bolts` the corresponding supergiant command would look like this:
`supergiant delete component command --app <your app name> --comp <your component name> --name <your container name> --cmd "/my-app" --cmd "--foo" --cmd "bar" --cmd "--nuts" --cmd "bolts"`
