
# 2D Space Shooter sample game (Unity NGO + Hathora Cloud)

[![UnityVersion](https://img.shields.io/badge/Unity%20Version:-2021.3%20LTS-57b9d3.svg?logo=unity&color=2196F3)](https://unity.com/releases/editor/qa/lts-releases#:~:text=February%2014%2C%202023-,LTS%20Release,2021.3.18f1,-Released%3A%20February)
[![NetcodeVersion](https://img.shields.io/badge/Netcode%20Version:-1.2.0-57b9d3.svg?logo=unity&color=2196F3)](https://docs-multiplayer.unity3d.com/netcode/current/about)
<br><br>

This sample game was started from Unity's [Netcode for GameObjects Bitesize Samples](https://github.com/Unity-Technologies/com.unity.multiplayer.samples.bitesize/tree/main/Basic/2DSpaceShooter)
<br><br>

### Overview

The original [2D Space Shooter Sample](https://github.com/Unity-Technologies/com.unity.multiplayer.samples.bitesize/tree/main/Basic/2DSpaceShooter) was a UNet sample that has been converted over to NGO. Check it out to learn more about physics movement and status effects using Netcode `NetworkVariables` and `ObjectPooling`. We have made a few modifications to make this game easily deployable with a dedicated server on [Hathora Cloud](https://hathora.dev/docs).
<br><br>

---
## Readme Contents and Quick Links
<details open> <summary> Click to expand/collapse contents </summary>

- ### [Getting the Project](#getting-the-project-1)
- ### [Requirements](#requirements-1)
- ### [Troubleshooting](#troubleshooting-1)
  - [Bugs](#bugs)
  - [Documentation](#documentation)

</details>

---
<br>

## Getting the project
### Direct download

 - select `Code` and select the 'Download Zip' option.  Please note that this will download the branch you're currently viewing on Github
<br><br>

## Requirements

This sample game is compatible with the latest Unity Long Term Support (LTS) editor version, currently [2021 LTS](https://unity.com/releases/2021-lts). Please include **Linux Dedicated Server Build Support** in your installation, as well as **Linux Build Support (Mono)**.

**PLEASE NOTE:** You will also need Netcode for Game Objects to use these samples. Complete the [Hello World](https://docs-multiplayer.unity3d.com/netcode/current/tutorials/helloworld) tutorial to prepare your environment.

You will also need to have an account created for Hathora Cloud (sign up at: https://console.hathora.dev)
<br><br>

## Steps to deploy and integrate Unity NGO game with Hathora Cloud
*Note: steps 1 - 3 have already been completed as part of this sample*

1. Add [Hathora Cloud Unity Plugin](https://github.com/hathora/unity-plugin) to your project
2. You must add a script to enable your dedicated server to automatically start in "Server" mode. See [NetworkCommandLine.cs](https://github.com/hathora/unity-ngo-2d-space-shooter/blob/main/src/Assets/Scripts/NetworkCommandLine.cs)
3. Then, attach the new script to the `NetworkManager` game object in the scene. This enable the script to listen for command line arguments configured (`-mode server`).
4. Use the Hathora Unity plugin to configure, build, and deploy your server on Hathora Cloud (for more detailed steps, check out [this guide](https://hathora.dev/docs/engines/unity/beginners-tutorial)).
5. Once deployed, create a room in Hathora Cloud (via plugin or [Hathora Console](https://console.hathora.dev)
6. Run your game client and enter in the connection information shown (note: you will need to convert the hostname to an IP address (i.e. `dig hnzpvf.edge.hathora.dev` in your terminal)


## Troubleshooting
### Bugs
- Report bugs in the sample game using Github [issues](https://github.com/hathora/unity-ngo-sample/issues)
  
### Documentation
For a deep dive into Hathora Cloud, visit our [documentation site](https://hathora.dev/docs).
<br><br>

## Community
For help, questions, advice, or discussions about Netcode for GameObjects and its samples, please join our [Discord Community](https://discord.gg/hathora). We have a growing community of multiplayer developers and our team is very responsive.
<br><br>

## Other samples
### Photon Fusion BR on Hathora Cloud
[Hathora Cloud + Photon Fusion Dedicated Server](https://github.com/hathora/hathora-photon-fusion-dedicated-server) is a minimal example of getting a dedicated server working with Photon Fusion.

### Hathora Unity Plugin
[Hathora Unity Plugin (with FishNet and Mirror demos)](https://hathora.dev/docs/engines/unity/beginners-tutorial) is our Unity Plugin that comes with FishNet and Mirror networking demos. It allows you to deploy your game on Hathora Cloud directly from our editor plugin.
<br><br>

