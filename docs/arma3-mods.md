---
id: arma3-mods
title: "Arma 3: Installation of Mods"
description: Information on installing mods on your Arma 3 game server from ZAP-Hosting - ZAP-Hosting.com Documentation
sidebar_label: Install Mods
services:
  - gameserver
---

import InlineVoucher from '@site/src/components/InlineVoucher';

## Introduction

Mods allow you to customize your server even more. The following explains where you can find the most popular server mods and how to set them up.

<InlineVoucher />

## Preparation

Through the [Steam Workshop](https://steamcommunity.com/app/107410/workshop/), you have the option to install mods on your server. The Steam Workshop is ideal for discovering and managing new and exciting mods. Start by browsing the Steam Workshop for mods that catch your interest. If you find a mod you like, it's important to note the associated Workshop ID. You can obtain the ID from the URL. This Workshop ID is necessary for the upcoming installation.



## Installation

The next step is to start installing the mods. Thanks to the Steam Workshop option, installation is straightforward. Access the management of your game server and navigate to Steam Workshop. There, you have the option to enter the mods into the provided field. Enter the Workshop IDs you have previously noted and add them there. If you are adding multiple mods, ensure that the mods are separated by a comma symbol.

![](https://screensaver01.zap-hosting.com/index.php/s/j8ki4CQ6MALAgcX/preview)

Following this, the mods need to be registered in the settings of your game server management. Enter the added mods into the Mods field and click Save.

![](https://screensaver01.zap-hosting.com/index.php/s/mBKesk6yFBFt35z/preview)

## What to Do When the Server Shows a Red Light

When you add multiple mods at once, such as `@mod1;@mod2;@mod3;@mod4;@mod5;@mod6;@mod7;@mod8;@mod9;@mod10;@mod11;@mod12`, sometimes the server may fail to load all the mods correctly. If this happens, the server management panel will show a red light instead of a green one, indicating an issue. This can also happen when a mod is faulty or hasn't been properly configured.

To avoid this, it's recommended to add mods in smaller batches. For example, start by adding `@mod1;@mod2;@mod3` and follow these steps:

1. **Save the server** → **Start the server** → **Check the server status** (Make sure it shows a green light)
2. **Stop the server** → Add more mods (`@mod4;@mod5`) → **Save the server** → **Start the server** → **Check the server status**

If the server shows a red light after adding more mods, it indicates an issue with the newly added mods. You can troubleshoot this by testing the mods one by one or switching the order, such as adding `@mod5` before `@mod4` to see which one is causing the issue.

### Key Application Issues
Another common reason for mods not functioning correctly is the lack of mod key application. Inside each mod folder, there’s usually a `keys` folder, which contains a `.bikey` file. This file needs to be placed in the `keys` folder of your server for the mod to be properly recognized and authenticated by the server. If you have installed 8 mods, you will need to add the corresponding 8 key files to the `keys` folder.

- If a red light appears after applying the mods, first check that the mod key files are correctly placed in the server’s `keys` folder.
- If the keys are already in place but the issue persists, the mod creator may not have updated the key file, or the mod itself may be faulty. In this case, it’s advisable to contact the mod creator via the **Steam Workshop** for further assistance.

### If the Red Light Appears for Only One Mod

If the red light shows for a specific mod, it often means that you forgot to apply the key file for that mod in the `keys` folder. Double-check if the key file for that mod is missing. If the key is present but the issue continues, the mod might be outdated or corrupted. In such cases, you may need to contact the mod creator or consider replacing the mod with a similar one.


## Conclusion

With the next server restart, the mods will be automatically downloaded, installed, and immediately available for use!
