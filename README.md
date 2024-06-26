[![npm version](https://badge.fury.io/js/angular2-expandable-list.svg)](https://badge.fury.io/js/angular2-expandable-list)
[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)

# YouTubePlayer Component

> The `YouTubePlayer` component is a customizable YouTube player built using React Native and the WebView component. It allows you to embed YouTube videos in your React Native application with various customization options.

## Prerequisites

This project requires NodeJS (version 8 or later) and NPM.
[Node](http://nodejs.org/) and [NPM](https://npmjs.org/) are really easy to install.
To make sure you have them available on your machine,
try running the following command.

```sh
$ npm -v && node -v
6.4.1
v8.16.0
```

## Table of contents

- [Project Name](#project-name)
  - [Prerequisites](#prerequisites)
  - [Table of contents](#table-of-contents)
  - [Getting Started](#getting-started)
  - [Installation](#installation)
  - [Usage](#usage)
    - [Serving the app](#serving-the-app)
    - [Running the tests](#running-the-tests)
  - [Contributing](#contributing)
  - [Authors](#authors)

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

## Installation

**BEFORE YOU INSTALL:** please read the [prerequisites](#prerequisites)


To install and set up the library, run:

```sh
$ npm install react-native-webview
$ npm i custom-rn-youtube-player
```

## Usage

### Serving the app

```sh
$ npm start
```

### Running the tests

```sh
$ npm test
```


Example:

```tsx
import React from 'react';
import { View } from 'react-native';
import YouTubePlayer from 'custom-rn-youtube-player';

const App = () => {
 const video_id='N3oCS85HvpY';
  return (
    <View>
      <YouTubePlayer
        videoSource={video_id}
        autoPlay={true}
        playButtonColor="#FF0000"
        hideYTLogo={true}
        hideTopBar={true}
        width="100%"
        height={300}
        onError={() => console.log('Error loading video')}
      >
      </YouTubePlayer>
    </View>
  );
};

export default App;

```

`props`

| Prop Name | Type | Default | Description|
| --- | --- | --- | --- |
| videoSource | String | "_CuSlwOmDOo" | The source URL or video ID of the YouTube video. |
| startVideoFrom | Number | 0| The time (in seconds) from which the video should start playing. |
| autoPlay |Boolean | false | Whether the video should start playing automatically. |
| playButtonColor | String |	"#000000" | 	The color of the play button. |
| hideYTLogo |Boolean | false |	Whether to hide the YouTube logo. |
| hideTopBar | Boolean | false |	Whether to hide the top bar of the player. |
| hideControls | 	Boolean | false |  Whether to hide the player controls. |
| hideCards | 	Boolean | false|	Whether to hide video suggestion cards. |
| width | 	String or Number |"100%" | 	The width of the player. |
|height | String or Number | 200 | 	The height of the player. |
| onError |Function | null | Callback function to handle errors. |



## Contributing


1.  Fork it!
2.  Create your feature branch: `git checkout -b my-new-feature`
3.  Add your changes: `git add .`
4.  Commit your changes: `git commit -am 'Add some feature'`
5.  Push to the branch: `git push origin my-new-feature`
6.  Submit a pull request :sunglasses:


## Authors

* **Sumit Nayak** 
