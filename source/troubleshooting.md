# Troubleshooting

Below are a list of common Supergiant issues and some resolution ideas for dealing with them.  Check back here often, as known or resolved issues will be added as we get more familiar with them.

## Dashboard (or other core services) aren't functioning properly

Sometimes a piece of the core services can experience a hiccup, or an install can occur during a brief version mismatch.  The first thing you can do to resolve this is to attempt a reinstall of those services:

```bash
supergiant delete core && supergiant create core
```

Under the hood this just disposes of all service containers, builds fresh ones and deploys them in your Supergiant system.
