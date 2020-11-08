---
id: choose-dev-env
title: Choose a Development Environment
---


----->>>>>> THE EXPLANATION IS NOT GGOD ENOUGH. ALSO - THIS ONLY SAYS THEY CAN CHOOSE THE REACT ENV. WHAT ABOUT MORE ENVS? OR CREATING THEIR OWN ENV? OR EXTENDING THIS ENV? THIS IS NOT GOOD ENOUGH


A [Bit Environment](/docs/environments/overview) is a component that configures and “bundles” together different services needed throughout the life-cycle of an independent component. These services include compiling, bundling, testing, linting, documenting, and more.

Bit environments make it possible to build and deliver independent components without the overhead of setting up a development environment to support that. Environments are also used to ensure consistency by standardizing the environment setup for independent components, developed across various (decoupled) repositories.
 
Bit provides a number of environments to choose from. Each of them is completely [customizable and extendible](/docs/environments/build-environment). 

We'll choose the [React environment](/docs/react/overview) by un-commenting `"teambit.react/react": { }` in the `workspace.jsonc` configuration file (produced in the previous step by initializing a new Bit workspace).

```json
  "teambit.workspace/variants": {

    "*": {

        "teambit.react/react": { }
    }

  }
```

A single workspace may use multiple environments to handle its different types of components. The above section demonstrates how to apply the React environment to all components in the workspace, using the `*` selector, inside the [variants](docs/variants/overview) field.
