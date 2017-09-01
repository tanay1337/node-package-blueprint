# Node Package Blueprint

[![Build Status](https://travis-ci.org/researchgate/node-package-blueprint.svg?branch=master)](https://travis-ci.org/researchgate/node-package-blueprint)
[![Codecov](https://img.shields.io/codecov/c/github/researchgate/node-package-blueprint.svg)](https://codecov.io/gh/researchgate/node-package-blueprint)
[![Dependency Status](https://dependencyci.com/github/researchgate/node-package-blueprint/badge)](https://dependencyci.com/github/researchgate/node-package-blueprint)

Simplify the creation and open sourcing of front-end projects.

- **👩‍💻&nbsp;&nbsp;Start From CLI:** generate the perfect starting blueprint for your new project
- **📐&nbsp;&nbsp;Project Layout**: follow a clear and pre-defined project structure to ease the way to open sourcing
- **🔧&nbsp;&nbsp;Integrated Tooling**: conciously chosen set of tools, configured and accessible via npm/yarn scripts
- **🎡&nbsp;&nbsp;Automated tasks**: from commit message checking to changelog generation for releases

We want to make the process of open source projects at [ResearchGate](https://github.com/researchgate) simple, and conventional.

When we create a new project, there are a lot of open questions around on how to best structure, document, and which tools to use.

This project provides the guidelines that clarify and facilitate this process.

## Getting started

Install Node Package Blueprint as a global npm package:

```
npm install -g @researchgate/node-package-blueprint
```

Now create a new project with the CLI tool:

```
node-package-blueprint my-project
cd my-project/
```

🏁&nbsp;&nbsp;Your project is ready! Take a look at the folder contents and when ready, install the dependencies:

```
yarn install
```

Once you're ready to release a new version use:

```
yarn release
```

This script will calculate the version number based on your commit history – make sure to follow the [conventional commits](conventionalcommits.org) guidelines. The [CHANGELOG.md](./CHANGELOG.md) file is automatically updated with the relevant changes.

If it's your first release, you probably do not want to bump a new version into the history.

In such cases, use the `--first-release` flag:

```
yarn release -- --first-release
```

## Documentation

Our documentation is structured in sections directly available under the `docs` folder:

- [How to Publish](./docs/docs/publishing.md)
- [Project Structure](./docs/docs/project-structure.md)
- [Integrated Tooling](./docs/docs/integrated-tooling.md)
- [Documenting on Github](./docs/docs/documenting-on-github.md)

## Contributing

We'd love to see your ideas and contributions to Node Package Blueprint. For more information about PRs and issues, see our [Contribution Guidelines](.github/CONTRIBUTING.md). Additionally, check out our [Code of Conduct](.github/CODE_OF_CONDUCT.md).