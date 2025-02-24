---
title: Holographic Remoting Overview
description: Learn about what Holographic Remoting is and how it can benefit your development process.
author: hferrone
ms.author: v-vtieto
ms.date: 9/8/2021
ms.topic: article
keywords: openxr, unity, hololens, hololens 2, mixed reality, MRTK, Mixed Reality Toolkit, augmented reality, virtual reality, mixed reality headsets, learn, tutorial, getting started, holographic remoting, desktop, preview
---

# Holographic Remoting Overview

You can use Holographic Remoting to stream holographic content to your HoloLens in real time. There are two main uses for this, and it's important to understand the difference:

1. (Unity or Unreal): **You want to preview and debug your app during the development process**: You can run your app locally in the Unity editor on your PC in Play Mode and stream the experience to your HoloLens. This provides a way to quickly debug your app without building and deploying a full project. We call this type of app a _Holographic Remoting Play Mode Preview app_.

    - [Learn more about previewing and debugging your app in **Unity**](../unity/preview-and-debug-your-app.md)

    - [Learn more about previewing and debugging your app in **Unreal**](../unreal/unreal-streaming.md)

1. (Unity, Unreal or C++):  **You want the resources of a PC to power your app instead of relying on the HoloLens on-board resources**: You can create and build an app that has Holographic Remoting capability. The user experiences the app on the HoloLens, but the app actually runs on a PC, which allows it to take advantage of the PC's more powerful resources. This can be especially helpful if your app has high-resolution assets or models and you don't want the frame rate to suffer. We call this type of app a _Holographic Remoting remote app_.

    - [Learn more about using PC resources in Unity](../unity/use-pc-resources.md)

    - [Learn more about using PC resources in Unreal](../unreal/unreal-streaming.md)

    - [Write a Holographic Remoting remote app using Windows Mixed Reality APIs (C++)](../native/holographic-remoting-create-remote-wmr.md)

    - [Write a Holographic Remoting remote app using OpenXR APIs (C++)](../native/holographic-remoting-create-remote-openxr.md)

In either case, inputs from the HoloLens--gaze, gesture, voice, and spatial mapping--are sent to the PC, content is rendered in a virtual immersive view, and the rendered frames are then sent to the HoloLens. 

## See Also

* [Holographic Remoting Player](holographic-remoting-player.md)
* [Tutorial: Getting started with PC Holographic Remoting](../unity/tutorials/mr-learning-pc-holographic-remoting-01.md)
* [Tutorial: Creating a Holographic Remoting PC application](../unity/tutorials/mr-learning-pc-holographic-remoting-02.md)
