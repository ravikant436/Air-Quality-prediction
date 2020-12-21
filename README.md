# Air-Quality-prediction
<a href="https://github.com/ravikant436/Air-Quality-prediction/commits/master" target="_blank">
  <img src="https://img.shields.io/github/last-commit/ravikant436/Air-Quality-prediction?style=flat-square" alt="GitHub last commit">
</a>

<a href="https://github.com/ravikant436/Air-Quality-prediction/issues" target="_blank">
  <img src="https://img.shields.io/github/issues/ravikant436/Air-Quality-prediction?style=flat-square&color=red" alt="GitHub issues">
</a>

<a href="https://github.com/ravikant436/Air-Quality-prediction/pulls" target="_blank">
  <img src="https://img.shields.io/github/issues-pr/ravikant436/Air-Quality-prediction?style=flat-square&color=blue" alt="GitHub pull requests">
</a>

<a href="https://github.com/ravikant436/Air-Quality-prediction#contribute" target="_blank">
  <img alt="Contributors" src="https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square">
</a>

<a href="https://standardjs.com" target="_blank">
  <img alt="ESLint" src="https://img.shields.io/badge/code_style-standard-brightgreen.svg?style=flat-square">
</a>
<hr>

Air quality is measure with the Air Quality Index(PM 2.5)

PM 2.5 is a fine particulate matter that is an air pollutant that is a concern for people’s health when levels in the air are high.

# Table of contents

- [Usage](#usage)
- [Development](#development)
    - [Data-Collection](#data-collection)
    - [Data-preprocessing](#data-preprocessing)
    - [Feature Importance](#feature-importance)
    - [Model Building](#model-building)
    - [Deployment](#deployment)
- [Conclusion](#conclusion)

# Usage

Install all dependencies. Run below command.
```sh
pip install -r requirements.txt
```
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
