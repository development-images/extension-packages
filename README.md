# VS Code Extension Packages

Various extension packs for my development environments.

The following requirements must be installed in the dev container for building new packages:

```bash
sudo npm install -g yo generator-code vsce
```

## Creating Extension Pack

To create an extension pack, create the new extension:

```bash
yo code
```

Add a publisher to the generated `package.json` file:

```bash
    "publisher": "gbe0",
```

## Building Package

Edit the package as needed.

Bump the version in `package.json` and add changelog entry.

Make sure that the personal access token is valid:

```bash
vsce login gbe0
```

Publish the extension:

```bash
vsce publish
```
