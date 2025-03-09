# Drag and Drop Grid Custom View ([@zsarnett](https://github.com/sponsors/zsarnett))

A testing ground and usable version of the Drag and Drop Grid that is being developed for Home Assistant Core Frontend.

Consider Subscribing to my YouTube Channel for updates on the Grid View: https://www.youtube.com/c/ZackBarett

## Installation
> :warning: The 2020.12 Release is recommended. Extra code for this was added to this release to make Drag and Drop better!

### Installation with `hacs`

1. Make sure the [HACS]([https://github.com/custom-components/hacs](https://github.com/yoely0966/Custom-Grid-View)) component is installed and working.
2. Add https://github.com/zsarnett/Custom-Grid-View as a custom repository
3. Add the configuration to your `ui-lovelace.yaml`

   ```yaml
   resources:
     - url: /hacsfiles/Custom-Grid-View/grid-view.js
       type: module
   ```

4. Refresh home-assistant.  

### Manual Installation

1. Download the `grid-view.js` file [Custom Drag and Drop Grid View]([[https://github.com/zsarnett/Custom-Grid-View/releases](https://github.com/yoely0966/Custom-Grid-View)](https://github.com/yoely0966/Custom-Grid-View))
2. Place the file in your `config/www` folder
3. Add a resource to your Lovelace Dashboard

   ```yaml
   title: Home
   resources:
     - url: /local/grid-view.js
       type: module
   ``` 

## How to use

To change the view to use Drag and Drop Grid, update the Lovelace YAML for that view and add

```yaml
type: custom:grid-dnd
```

### Example

```yaml
path: default_view
type: 'custom:grid-dnd'
title: Home
cards: []
```

> :warning: **I recommend copying your view and modifying the copy instead of modifying your existing dashboard**

> :warning: **Users using YAML mode only will not have a good time :)**

### Notes

* This is not the finished version
* This version is not the best version
* This view is bound to change and have breaking changes
* This will add a large amount of YAML to your view. `layout: {}`
* This will add a key to every card.
* Again its not perfect and I will try to update this version as I find better ways.


* I have built the everything that this code is using. ie. Lit-Grid-Layout
   * This means I have complete control over the changes which is good
   * This also means it may not be the best yet. I am still learning even after 2 years of working with Home Assistant. I will try to perfect the code as you all and myself test this view
 


** PLEASE BE PATIENT WITH ME ON THIS :smile: **

Add any bugs that you find as issues in this repo. 

THANK YOU!

Consider Sponsoring me as this helps me find the time to develop this! Thank you: https://github.com/sponsors/zsarnett


Known Issues:

* You can not have empty space between cards
* Sometimes the place holder isn't aligned correctly
* Some Cards do not support resizing 
* Not Mobile Friendly
