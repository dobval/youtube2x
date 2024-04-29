<p align="center">
<img src="https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E">
</p>
<img alt="Static Badge" src="https://img.shields.io/badge/License-MIT-green">

# youtube2x

Simple script to set the playback of youtube videos to 2x automatically.

## Installation/Usage
Due to me not simply not wanting to publish it to Firefox or Chrome add-on store,
one can freely publish it and give credit according to the MIT license or load it locally, see further below.

### Firefox

I prefer to add it as a temporary addon because it is easier:

1. Enter `about:debugging` in the URL bar.
2. Click on *This Firefox*.
3. Click on *Load Temporary Add-on*.

However here is another way to install the local addon in Firefox:

1. Navigate to `about:config` in Firefox.
2. Set `xpinstall.signatures.required` to `false`. This allows the installation of unsigned addons.
3. Add an explicit id to `browser_specific_settings` section in the manifest. For example:
    ```json
    "browser_specific_settings": {
      "gecko": {
        "id": "your-addon@your-domain"
      }
    }
    ```
4. Pack the extension into a `.xpi` file. You can do this by simply renaming the downloaded `.zip` file extension to `.xpi`.
5. Go to the Add-ons Manager (`about:addons`), click on the gear icon, choose `Install Add-on from file` and select your `.xpi` file.

### Chrome

Follow these steps to load your local addon in Chrome:

1. Open the Extension Management page by navigating to `chrome://extensions`.
2. Enable Developer Mode by clicking the toggle switch next to `Developer mode`.
3. Click the `LOAD UNPACKED` button and select the extension directory.
