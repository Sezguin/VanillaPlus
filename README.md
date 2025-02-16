# VanillaPlus
A Minecraft modpack for an enhanced vanilla experience.

## Prerequisites

1. You are running Windows.
2. Your Minecraft Launcher is installed and updated to the latest version.
3. You have the latest version of Java installed. Go to [this link](https://www.java.com/download/ie_manual.jsp) if you do not.
4. You can read.

## Installation Guide

### Setting Up Iris and Fabric

*Before starting these steps, make sure your Minecraft Launcher is closed and Minecraft is not running.*

1. Go to the Iris Shaders website and download the Universal Jar from [this link](https://www.irisshaders.dev/download).
2. This should download a `.jar` file. Double click this to launch the installer (if you can't do this, double check you've installed Java correctly as per step 2 of the pre-requisites).
3. The installer should now launch. Select version **1.21.1** and make sure you've selected to install **both Iris and Fabric**.
4. Once the installation has completed, exit the Iris installer.
5. Now boot up the Minecraft Launcher. You should see that it's defaulted to the `Fabric Loader 1.21.1` version of the game. Do not click play yet.
6. Go to the `Installations` tab on the Minecraft launcher. Click the three dots next to the `Fabric Loader 1.21.1` installation and click **edit**.
7. Scroll down and click the dropdown `More Options` - you should see a section for `JVM arguments` at the very bottom.
8. At the start of the text box, you'll see something like `-Xmx2G`. Change the `2G` to the number that is **half the total RAM on your system**. For example, if you have 32GB of RAM, you should change `-Xmx2G` to `-Xmx16G`.
9. Click Save.
10. Switch back to the `Play` tab on the Minecraft launcher, double check that `Fabric Loader 1.21.1` is still selected in the bottom left, and click **Play**.
11. Once the game has loaded successfully, close it down and move to the next step.

### Installing the Mods

*For the next steps, you will need to download this repository from GitHub in order to use the files within it. Click the green `Code` dropdown on the page and then `Download ZIP`. Once downloaded, extract the contents to a folder for access.*

1. After extracting this repository locally, navigate to the `Mods` folder and copy **everything**.
2. Navigate to your `.minecraft` installation. *For a quick way to do this, press the **Windows Key and R at the same time** to bring up a Run box (which will appear in the bottom left of your screen), the type `%appdata%` into the box and click run. This will take you to your Roaming folder, and you should see the `.minecraft` folder near the top.*
3. Paste all the mods you copied from step 1 into the `Mods` folder. There should be two in there already - leave these as they are.

*The following steps are optional but **HIGHLY RECOMMENDED** for an improved visual experience.*

### Installing Shader Packs

*These 3 shader packs have been specifically chosen as they are compatible with the Distant Horizons mod.*

1. In the repository you downloaded earlier, there is a `Shaderpacks` folder containing 3 shaderpack ZIPs. Copy these 3 `.zip` files and place them in the `shaderpacks` folder in your `.minecraft` installation folder. Follow the previous step 2 of 'Installing the Mods' to navigate to this folder again if you need to.

### Installing the Resource Pack

1. Similar to the shaderpacks, there is a `Resourcepacks` folder in the repository you downloaded. Copy that `Simplista.zip` file and paste it in the `resourcepacks` folder in your `.minecraft` installation.

### First Time Launch and Configuration

*You can now launch the game and play, but there's a little more configuration to do first.*

1. Open up your Minecraft Launcher and click play. Again, make sure `Fabric Loader 1.21.1` is selected in the bottom left.
2. Once you are loaded in, go to `Options` then `Resource Packs` and make sure the `Simplista` resource pack had been added to your selected packs. Click **Done** and wait for the changes to apply.
3. Next, go back to the main menu and navigate to `Options` then `Video Settings` then `Shader Packs`.

*There are 3 shader packs to choose from, I highly recommend `Complementary Unbound`.*

4. Click once on the shader pack you want to use, then click **Apply**. Wait for the changes to take effect.

**You will also need to change some default video settings.**

1. Go to `Options` then `Video Settings`.
2. `Render Distance` should be no more than **14**. (Reduce for better performance).
3. `Simultion Distance` should be no more than **12**
4. `Brightness` should be maximum (bright).
5. Under the `Quality` settings, make sure `Graphics`, `Clouds`, `Weather` and `Leaves` are all set to **Fancy**.

That it, you're now done and can play. There are some more settings to configure in the shaderpack options if you want to, but these are personal preference and now required - though they do (in my opinion) enhance the experience.

**YOU CAN NOW ASK SEZGUIN FOR THE SERVER INFORMATION TO JOIN.**

### Optional Shader Pack Configuration

*Note: This is only for the Complementary Unbound Shaders. If you are using a different pack, this does not apply.*

1. From the in-game Minecraft menu, go to `Options` -> `Video Settings` -> `Shader Packs`.
2. Ensure Complementary Unbound is selected then go to `Shader Pack Settings`.
3. Go to `Materials` then `IntegratedPBR+ Materials` and change `Generated Normals` to **ON** and `Coated Textures` to **ON**.
4. Next, fo back to the main shader pack options menu and go to the `Atmosphere` options.
5. Go to `Clouds` and change `Cloud Shadows` to **ON**. Change `Cloud Altitude` to something higher than **300** (unless you want clouds clipping through the tops of mountains, which can be nice - experiement with this) and finally go to the `Unbound Cloud Settings` options and increase the `Cloud Amount`, `Cloud Smallness` and `Rain Cloud Addition` by a small amount. Mine are on `1.2`, `1.1` and `+1.00` respectively.

*These are personal preference and worth experimenting with. If you change too much and don't like it, you can reset the shader pack to its defaults.*

### Optional Distant Horizons Configuration

1. Go to `Options` from your in-game Minecraft menu.
2. You should see an icon next to the FOV slider that looks like some squares within squares.
3. Ensure `Enable Rendering` and `Enable Cloud Rendering` are set to **True**.
4. `LOD Chunk Render Distance Radius` should be between 128 - 512 (this is how far you can see, feel free to experiment) - mine is on 512 for maximum view distance.
5. `Quality Preset` should be **High** or **Extreme** - but play around for best performance.

### Optional Distant Horizons Data Transfer

*For this step, make sure Minecraft is not running.*

One of the mods included in this pack is the Distant Horizons mod. This enabled you to see extremely far in the distance with minimal impact on your system.

The issue with running this on a server, is that you must explore the chunks first before they can remain generated.

To solve this, I've pre-generated a large amount of the initial starting area so you don't have to.

1. Sezguin should have included a Link to Google Drive for the Distant Horizons Data when sending you this guide. If not, ask.
2. Go to the Drive link, and download the file.

*It's quite large, so give it time to download.*

3. Once downloaded, copy the file and navigate to your Minecraft installation folder. Use a previous reference to get here if you need to.
4. There should be a `Distant_Horizons_server_data` folder. Go in here, then to `Mount+Sirgophagus`, then `overworld` and **DELETE** the existing `DistantHorizons.sqlite` file.
5. Paste the file you downloaded from Google Drive here.
6. Launch the game and enjoy the beautiful landscapes.

That's it, you should now be ready to play - if you've made it this far, then fair play for reading through all this.

*Reach out to Sezguin if you get stuck or have any questions.*
