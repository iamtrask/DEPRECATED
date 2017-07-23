# How-To update charts

## installation

Make sure you got NodeJS installed and install the dependencies with

```sh
npm install
```

## usage

The sourcecode for the charts used in the [readme](readme.md) are stored in [./src](src) and are in [mermaid](http://knsv.github.io/mermaid) syntax. After modifying the sourcecode you need to recompile them manually (as of now) and reference them in the readme. To compile all the source files run `npm run dist` in this directory.

_Note: If you decide to delete a source file, please remove the corresponding compiled **png** file as well_
