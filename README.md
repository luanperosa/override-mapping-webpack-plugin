# Override Mapping Webpack Plugin

This plugin is used on PWA Studio project. It helps you to override components/files.

# Usage

```
    npm i override-mapping-webpack-plugin-pwa-studio
```

Import it as a new plugin on your `webpack.config.js` file.

```
const OverrideMappingPlugin = require('override-mapping-webpack-plugin-pwa-studio');

clientConfig.plugins.push(new OverrideMappingPlugin({
    // Insert here the map that you need to override. It will be like this:
    '@magento/venia-ui/lib/components/Header/header.css': 'src/lib/components/Header/header.css',
}));
```
