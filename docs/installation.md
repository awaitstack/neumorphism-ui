---
sidebar_position: 1
---

# Installation

**Neumorphism UI** is supported in React Native CLI initiated apps. For Expo projects is coming soon.

## Getting Started

Open a Terminal in your project's folder and run:

```bash
npm install neumorphism-ui
```

or

```bash
yarn install neumorphism-ui
```

### What you'll need

- [Nodejs](https://nodejs.org/en/download/) version 14 or above:
  - When installing Node.js, you are recommended to check all checkboxes related to dependencies.

- [Yarn](https://yarnpkg.com/getting-started/install) latest version:
  - When installing Yarn, you are recommended to check all checkboxes related to dependencies.

## Usage

Wrap your root component in **NeumorphismProvider** from `neumorphism-ui`. If you have a vanilla React Native project, it's a good idea to add it in the component which is passed to `AppRegistry.registerComponent`. This will usually be in the `index.js` file like the example below:

```tsx
import * as React from 'react';
import {AppRegistry} from 'react-native';
import {NeumorphismProvider} from 'neumorphism-ui';
import {name as appName} from './app.json';
import App from './src/App';

AppRegistry.registerComponent(appName, () => (
  <NeumorphismProvider>
    <App />
  </NeumorphismProvider>
));
```

The **NeumorphismProvider** component provides the theme to all the components in the framework.

## Customization

You can provide a custom theme to customize the colors. with the `NeumorphismProvider` component. Check the [default theme](https://github.com/awaitstack/neumorphism-ui/blob/main/src/styles/DefaultTheme.tsx) to see what customization options are supported.

```tsx
import * as React from 'react';
import { DefaultTheme, NeumorphismProvider } from 'neumorphism-ui';
import App from './src/App';

const theme = {
  ...DefaultTheme,
  colors: {
    ...DefaultTheme.colors,
    primary: 'red',
    accent: 'yellow',
  },
};

export default function Main() {
  return (
    <NeumorphismProvider theme={theme}>
      <App />
    </NeumorphismProvider>
  );
}
```
