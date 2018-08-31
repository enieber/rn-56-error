# React Native Error in 0.56.0

I build this project to reproduce error in init project with react-native init

react-native -version

**$ react-native --version**

- react-native-cli: 2.0.1

- react-native: 0.56.0


Error in run project, message:

```
error: bundling failed: Error: Unable to resolve module `AccessibilityInfo` from `project_name\node_modules\react-native\Libraries\react-native\react-native-implementation.js`: Module `AccessibilityInfo` does not exist in the Haste module map

This might be related to https://github.com/facebook/react-native/issues/4968
To resolve try the following:
  1. Clear watchman watches: `watchman watch-del-all`.
  2. Delete the `node_modules` folder: `rm -rf node_modules && npm install`.
  3. Reset Metro Bundler cache: `rm -rf /tmp/metro-bundler-cache-*` or `npm start -- --reset-cache`.  4. Remove haste cache: `rm -rf /tmp/haste-map-react-native-packager-*`.
    at ModuleResolver.resolveDependency (C:\project_name\node_modules\metro\src\node-haste\DependencyGraph\ModuleResolution.js:167:1306)
    at ResolutionRequest.resolveDependency (C:\project_name\node_modules\metro\src\node-haste\DependencyGraph\ResolutionRequest.js:80:16)
    at DependencyGraph.resolveDependency (C:\project_name\node_modules\metro\src\node-haste\DependencyGraph.js:237:485)
    at Object.resolve (C:\project_name\node_modules\metro\src\lib\transformHelpers.js:116:25)
    at dependencies.map.result (C:\project_name\node_modules\metro\src\DeltaBundler\traverseDependencies.js:298:29)
    at Array.map (<anonymous>)
    at resolveDependencies (C:\project_name\node_modules\metro\src\DeltaBundler\traverseDependencies.js:294:16)
    at C:\project_name\node_modules\metro\src\DeltaBundler\traverseDependencies.js:159:33
    at Generator.next (<anonymous>)
    at step (C:\project_name\node_modules\metro\src\DeltaBundler\traverseDependencies.js:239:307)

```
