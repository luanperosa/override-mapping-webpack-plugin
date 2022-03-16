# Override Mapping Webpack Plugin

This plugin is used on PWA Studio project. It helps you to override components/files.

# Usage

```
$ yarn add -D bitbucket:webjump/override-mapping-webpack-plugin
```

Import it as a new plugin on your `webpack.config.js` file.

```
const webjumpOverrideMappingPlugin = require('override-mapping-webpack-plugin');

clientConfig.plugins.push(new webjumpOverrideMappingPlugin({
    // Insert here the map that you need to override. It will be like this:
    '@magento/venia-ui/lib/components/Header/header.css': 'src/lib/components/Header/header.css',
}));
```
