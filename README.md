# &#60;dsc-polymer-video-bg&#62;

[![Build Status](https://travis-ci.org/discovery-tecnologia/dsc-polymer-video-bg.svg?branch=master)](http://travis-ci.org/#!/discovery-tecnologia/dsc-polymer-video-bg)
[![npm](https://img.shields.io/npm/l/express.svg)]()

Allows you to set videos as background in HTML.

Suported formats: mp4, webm, ogg and ogv.

Large videos can denigrate the user experience. We recommend the use of videos of short duration and with optimized compression.
Newer versions of Chrome have a tool for testing connection speed limitation. This can be useful for simulating loading videos in production.
To access go to the Developer Tools and the Network tab select the desired speed in the last selector at the top right.

Diferentials:

 * Responsive
 * Fallback souce video formats
 * Background image fallback
 * Custom content
 * Custom styling

## Demo

```
$ git clone https://github.com/discovery-tecnologia/dsc-polymer-video-bg.git
$ cd dsc-polymer-video-bg
$ npm install
$ node install -g polymer-cli
$ polymer serve
```
Open browser: http://localhost:8080/components/dsc-polymer-video-bg/demo/

## Usage

Install with:

```
$ bower i dsc-polymer-video-bg --save
```

Example usage:

```html
<dsc-polymer-video-bg src='["videos/video.mp4", "videos/video.webm", "videos/video.ogg"]'>
  <h1>Background video HTML element</h1>
</dsc-polymer-video-bg>
```

## API

| Property       | Description                            | Type   | Default    |
|:---------------|----------------------------------------|--------|------------|
| srcs           | List of sources. mp4, webm, ogg or ogv | Array  | []         |
| background     | Background image until video dowload.  | String | ""         |
| muted          | Turns off video sound                  | String | ""         |

Accepts any HTML content.

The content can be any HTML element or other polymer component.

| Custom property                |	Description                             | Default |
|:-------------------------------|------------------------------------------|---------|
| --dsc-polymer-video-bg         | Overhide root element style              | {}      |
| --dsc-polymer-video-bg-content | Overhide the content container style     | {}      |
| --dsc-polymer-video-bg-overlay | Set overlay element style                | {}      |

## Test

Check sintax and execute selenium tests.

```
$ npm test
```
