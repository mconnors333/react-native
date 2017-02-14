# React-Native
The Greatest Most Awesomest Tech Demo in the ENTIRE UNIVERSE!

## What is React-Native?

React Native lets you build mobile apps using only JavaScript. It uses the same design as React, letting you compose a rich mobile UI from declarative components.

## Where to Begin

First we are going to ensure our Node and Watchman are up-to-date by running the following.

```
brew install node
```
```
brew install watchman
```
Next, we have to install the React-Native CLI with the following command

```
npm install -g react-native-cli
```

Lastly, in order to develop for IOS it requires an up-to-date version of Xcode.  Android requires an up-to-date version of Android Studio.

## Starting the Project

Run the following commands to create a new React-Native app.

```
react-native init AwesomeProject
```
```
cd AwesomeProject
```
```
react-native run-ios
```
Once Simulator and Atom has finished loading.  Open the index.ios.js file for editing.

## Using Props

Props are used in the same way as regular React

```
import React, { Component } from 'react';
import { AppRegistry, Text, View } from 'react-native';

class Greeting extends Component {
  render() {
    return (
      <Text>Hello {this.props.name}!</Text>
    );
  }
}

class LotsOfGreetings extends Component {
  render() {
    return (
      <View style={{alignItems: 'center'}}>
        <Greeting name='Matthew' />
        <Greeting name='Sandy' />
        <Greeting name='Julie' />
      </View>
      );
}
}

AppRegistry.registerComponent('AwesomeProject', () => LotsOfGreetings);
```
