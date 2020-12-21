# Air-Quality-prediction

<p align="center">
  <a href="https://github.com/ravikant436/Air-Quality-prediction/releases/" target="_blank">
    <img alt="GitHub release" src="https://img.shields.io/github/v/release/ravikant436/Air-Quality-prediction?include_prereleases&style=flat-square">
  </a>

  <a href="https://github.com/ravikant436/Air-Quality-prediction/commits/master" target="_blank">
    <img src="https://img.shields.io/github/last-commit/ravikant436/Air-Quality-prediction?style=flat-square" alt="GitHub last commit">
  </a>

  <a href="https://github.com/ravikant436/Air-Quality-prediction/issues" target="_blank">
    <img src="https://img.shields.io/github/issues/ravikant436/Air-Quality-prediction?style=flat-square&color=red" alt="GitHub issues">
  </a>

  <a href="https://github.com/ravikant436/Air-Quality-prediction/pulls" target="_blank">
    <img src="https://img.shields.io/github/issues-pr/ravikant436/Air-Quality-prediction?style=flat-square&color=blue" alt="GitHub pull requests">
  </a>

  </br>

  <a href="https://github.com/ravikant436/Air-Quality-prediction#contribute" target="_blank">
    <img alt="Contributors" src="https://img.shields.io/badge/all_contributors-10-orange.svg?style=flat-square">
  </a>

  <a href="https://standardjs.com" target="_blank">
    <img alt="ESLint" src="https://img.shields.io/badge/code_style-standard-brightgreen.svg?style=flat-square">
  </a>
</p>
<hr>

A Google Chrome/Firefox extension that blocks NSFW images from the web pages that you load using TensorFlowJS.

*This extension **does NOT** collect/send any user data. All the operations on the images are done locally on the browser. No user data is being sent to a server for processing.*

<p align="center">
  <img alt='logo name' src='./demo/images/logo_name.png'>
</p>

<p align="center">
  <img alt="GitHub release" src="https://raw.githubusercontent.com/nsfw-filter/nsfw-filter/master/demo/images/demo_v3.gif">
</p>

When a web page is loaded, all the images remain hidden until they are found to be NSFW or not. If they are found to be NSFW, they remain hidden. Otherwise, they become visible.

It is free and is currently supported on both Chrome and Firefox. We are working on porting this to Safari also.
</br>
<p align="center">
  <a href="https://chrome.google.com/webstore/detail/nsfw-filter/kmgagnlkckiamnenbpigfaljmanlbbhh" target="_blank">
    <img src="./demo/images/chrome.gif" alt="Download now" width="160">
  </a>
  <a href="https://addons.mozilla.org/en-US/firefox/addon/nsfw-filter/" target="_blank">
    <img src="./demo/images/firefox.gif" alt="Download now" width="160">
  </a>
</p>

<p align="center">
<a href="https://chrome.google.com/webstore/detail/nsfw-filter/kmgagnlkckiamnenbpigfaljmanlbbhh" target="_blank"><strong>Download for Chrome</strong></a> | <a href="https://addons.mozilla.org/en-US/firefox/addon/nsfw-filter/" target="_blank"><strong>Download for Firefox</strong></a>
</p>

Read about the release in [**Hacker Noon**](https://hackernoon.com/nsfw-filter-introduction-building-a-safer-internet-using-ai-jq1e3u2f) or in [**Towards Data Science**](https://towardsdatascience.com/building-a-safer-internet-for-everyone-using-ai-175df5e02cee).

Model used - [**nsfwjs**](https://github.com/infinitered/nsfwjs) developed by [**Infinite Red, Inc.**](https://github.com/infinitered)

Reach out to us! Join the [**Slack channel**](https://join.slack.com/t/nsfwfilter/shared_invite/zt-gt1lgdiv-K2VR~UVUxwaTPWCLSmDiug).

# Table of contents

- [Usage](#usage)
- [Development](#development)
    - [Adding to Chrome](#adding-to-chrome)
    - [Adding to Firefox](#adding-to-firefox)
- [Contribute](#contribute)

# Usage

After adding the extension to Chrome/Firefox, it will light-up everytime you load a compatable website.

When a page is loaded, the extension would hide all the images in the page and only show images that have been classified as **NOT NSFW**.

You can toggle(off/on) the extension from the ```chrome://extensions``` page in Chrome and ```about:debugging#/runtime/this-firefox``` in Firefox.

Open popup window to change NSFW Filter settings

<table>
  <tr>
    <td vlign="center">
      <img src="./demo/images/pin_popup.png" alt="Pin popup window">
    </td>
    <td vlign="center">
      <img src="./demo/images/popup.png" alt="Popup window">
    </td>
  </tr>
</table>


# Development

Clone this repository and navigate inside the project folder and install the dependencies by running:

```sh
npm ci
```

After installing the dependencies, build the project by executing:

```sh
npm run build
```

Run the tests

```sh
npm run test
```

### Adding to Chrome

To install the developer version follow the steps below. To just use the extension download from [**chrome.google.com/webstore/nsfw-filter**](https://chrome.google.com/webstore/detail/nsfw-filter/kmgagnlkckiamnenbpigfaljmanlbbhh)

To run development version in clean environment use command:

```sh
npm run dev:chrome
```

Or open Google Chrome and open the Extension Management page by navigating to ```chrome://extensions``` or by opening Settings and clicking Extensions from the bottom left.

Enable Developer Mode by clicking the toggle switch next to Developer mode.

Click the "Load Unpacked" button and select the extension directory(```.../dist```).

<p align="center">
  <img src="./demo/images/install_instructions.png" alt="Install Instructions">
<p/>

Voila! The extension is now installed and ready to be used!

### Adding to Firefox

To install the developer version follow the steps below. To just use the extension download from [**addons.mozilla/nsfw-filter**](https://addons.mozilla.org/en-US/firefox/addon/nsfw-filter/)

To run development version in clean environment use command:

```sh
npm run dev:firefox
```

Or open Firefox and open the Debug Add-ons page by navigating to ```about:debugging#/runtime/this-firefox``` or by selecting it from Settings dropdown in the add-ons page.

Click Load Temporary Add-on and select the ```manifest.json``` file from the ```.../dist``` directory.

<p align="center">
  <img src="./demo/images/install_instructions_firefox.png" width="470px" alt="Install Instructions">
<p/>

That's it! The extension is now ready to be used in Firefox!
<!--
### Activity Diagram

![](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.githubusercontent.com/nsfw-filter/nsfw-filter/master/demo/UML/activity-diagram.plantuml)
-->
# Contributor
<table>
  <tr>
    <td align="center"><a href="https://github.com/ravikant436"><img src="https://github.com/ravikant436/ravikant436.github.io/blob/main/images/photo-1.jpeg" width="100px;" alt=""/><br /><sub><b>Ravikant Tyagi</b></sub></a><br /></td>
  </tr>
</table>
