# Custom SABnzbd integration for Home Assistant
Due to a breaking change in Home Assistant 2022.3, the SABnzbd integration has stopped working as the Python package it depends on uses the loop keyword argument.

I have created this custom component as a temporary workaround until the official integration is fixed.

All credit goes to DavidFW1960 for the custom component configuration and the `manifest.json` and thank you to tkdrob for providing the fix for pysabnzbd!

The relevant issues/conversations in the Home Assistant repository are:

https://github.com/home-assistant/core/issues/61306
https://github.com/home-assistant/core/issues/67532

## Installation
_The below steps assume you have [HACS](https://hacs.xyz/) installed_
1. Navigate to HACS (click HACS on the sidebar!)
2. Open Integrations
3. Click the three little dots in the top right hand corner and select "Custom repositories"
4. Paste the URL of this repository into the "Repository" text box
5. Select the category "Integrations"
6. Click "Add"
7. Press the blue `+` icon in the bottom right hand corner
8. Search for "Custom SABnzbd", select it and click "Download this repository with HACS" & click "Download" on the following popup
9. Reload Home Assistant Core and the SABnzbd integration will work as it did before 2022.3
