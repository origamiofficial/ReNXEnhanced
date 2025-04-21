# ReNXEnhanced

**A lightweight Tampermonkey script for importing and exporting NextDNS configuration profiles.**

![Static Badge](https://img.shields.io/badge/Install_this_script-Tampermonkey-blue?color=%2300485b&link=https%3A%2F%2Fraw.githubusercontent.com%2Forigamiofficial%2FReNXEnhanced%2Frefs%2Fheads%2Fmain%2FReNXEnhanced.user.js) ![We Support](https://img.shields.io/badge/we%20stand%20with-%F0%9F%87%B5%F0%9F%87%B8%20palestine-white.svg)

---

## Introduction

**ReNXEnhanced** is a streamlined userscript designed to simplify the management of NextDNS configuration profiles. Built upon the foundation of the original [NXEnhanced](https://github.com/hjk789/NXEnhanced) web extension by [hjk789](https://github.com/hjk789), this script focuses exclusively on the essential functionality of importing and exporting configuration profiles. It integrates seamlessly with the NextDNS website, providing a lightweight and efficient solution for users who need to manage their DNS settings without the overhead of additional features.

---

## Features

- **Import NextDNS Configuration**: Easily import configuration profiles directly into your NextDNS account.
- **Export NextDNS Configuration**: Export your current NextDNS configuration for backup or sharing.
- **Lightweight and Efficient**: Stripped of unnecessary features, ReNXEnhanced is optimized for performance and ease of use.
- **Seamless Integration**: Dynamically adds import and export buttons to the NextDNS settings page for a native experience.

---

## Installation

To use ReNXEnhanced, you'll need a userscript manager like [Tampermonkey](https://www.tampermonkey.net/). Follow these steps to install the script:

1. **Install Tampermonkey**:
   - If you haven't already, install the Tampermonkey extension for your browser from [here](https://www.tampermonkey.net/).

2. **Install the Script**:
   
   - ![Static Badge](https://img.shields.io/badge/Install_this_script-Tampermonkey-blue?color=%2300485b&link=https%3A%2F%2Fraw.githubusercontent.com%2Forigamiofficial%2FReNXEnhanced%2Frefs%2Fheads%2Fmain%2FReNXEnhanced.user.js)

4. **Verify Installation**:
   - Visit [my.nextdns.io](https://my.nextdns.io/).
   - Navigate to the settings page to see the newly added "Export this config" and "Import a config" buttons.

---

## Usage

Once installed, ReNXEnhanced enhances the NextDNS settings page with two new buttons:

- **Export this config**: Click this button to download your current NextDNS configuration as a JSON file.
- **Import a config**: Click this button to upload and apply a previously exported configuration file.

### How to Export a Configuration

1. Navigate to the settings page on [my.nextdns.io](https://my.nextdns.io/).
2. Click the "Export this config" button.
3. Save the generated JSON file to your desired location.

### How to Import a Configuration

1. Navigate to the settings page on [my.nextdns.io](https://my.nextdns.io/).
2. Click the "Import a config" button.
3. Select the JSON configuration file you wish to import.
4. Wait for the import process to complete, and the page will reload with the new settings applied.

---

## Technical Details

### Adaptation from NXEnhanced Web Extension

ReNXEnhanced was created by extracting and refining the core import and export logic from the original [NXEnhanced](https://github.com/hjk789/NXEnhanced) web extension. The adaptation process involved several key modifications to ensure compatibility and efficiency within the Tampermonkey environment:

- **Environment Tailoring**: The script was adjusted to operate within the constraints of a userscript, which runs in a more limited context compared to a full web extension. This required rewriting parts of the code to leverage Tampermonkey's APIs and the browser's DOM manipulation capabilities.
- **Functionality Focus**: All non-essential features from the original extension, such as log counters and tooltips, were removed to concentrate solely on configuration management. This reduction streamlined the codebase and improved execution speed.
- **API Interactions**: The script directly interfaces with the NextDNS API to fetch and update configuration data, using `fetch` requests to handle JSON payloads. This ensures that only the necessary data is processed, minimizing overhead and maintaining compatibility with NextDNS's infrastructure.
- **UI Integration**: The import and export buttons are dynamically injected into the NextDNS settings page using JavaScript DOM manipulation. This approach ensures a consistent and intuitive user interface without requiring a full extension framework.

### Differences from the Original Web Extension

While ReNXEnhanced is derived from NXEnhanced, there are several notable differences:

- **Scope**: ReNXEnhanced is narrowly focused on configuration import and export, whereas NXEnhanced offers a broader range of features, including log management and security enhancements. This focused scope makes ReNXEnhanced a specialized tool for config management.
- **Installation Method**: As a userscript, ReNXEnhanced requires a userscript manager like Tampermonkey, whereas NXEnhanced is installed as a standalone web extension directly in the browser. This impacts the deployment model and user prerequisites.
- **Performance**: By stripping away extraneous features, ReNXEnhanced is lighter and more efficient, with a reduced memory footprint and faster execution time. This makes it ideal for users who only need configuration management capabilities.
- **Codebase**: The userscript version has a significantly reduced codebase, containing only the essential logic for import and export operations. This contrasts with NXEnhanced's more comprehensive codebase, which supports multiple functionalities.

---

## Acknowledgments

- **Original Author**: Special thanks to [hjk789](https://github.com/hjk789) for creating the original [NXEnhanced](https://github.com/hjk789/NXEnhanced) web extension, which served as the foundation for this userscript.

---

## License

This project is licensed under the [MIT License](LICENSE), allowing for free use, modification, and distribution.

---

## Warning
Use of this script may constitute a breach of the [NextDNS Terms of Service](https://help.nextdns.io/terms). Use at your own risk.

[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/origamiofficial/ReNXEnhanced&icon=github.svg&icon_color=%23FFFFFF&title=hits&edge_flat=false)](https://github.com/origamiofficial/ReNXEnhanced)