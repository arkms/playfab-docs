---
title: Azure PlayFab SDKs
author: joannaleecy
description: Azure PlayFab SDKs
ms.author: joanlee
ms.date: 02/22/2021
ms.topic: article
ms.service: playfab
keywords: playfab, playfab sdk
ms.localizationpriority: medium
---

# PlayFab Services SDK

The PlayFab Services SDKs are organized below by language, platform, and game engine to help you find the right SDK for your project.

PlayFab Services SDKs enable you to implement all of the PlayFab features not explicitly called out in one of our [other SDKs](sdk-overview.md), including LiveOps, economy, and data analytics.

Access to SDKs for Nintendo Switch, PlayStation&#174;4, and PlayStation&#174;5 requires special approval and adherence to platform policies. For more information, see [Request access for SDKs and samples](../features/multiplayer/networking/request-access-for-sdks-samples.md).

For broad API categories in these SDKs, see [API REST operation groups](/rest/api/playfab/admin/).

> [!TIP]
> Unsure if this is the SDK you need? See [SDK overview - PlayFab SDK, Party SDK, Multiplayer Server SDK](sdk-overview.md).

"PlayStation" is a registered trademark or trademark of Sony Interactive Entertainment Inc.

## By language

| Language                          | Platform/environments                     |
|-----------------------------------|-------------------------------------------|
| C/C++                             | [Windows (Win32)](c/index.md), [GDK (Xbox and Windows)](c/index.md), [Switch](https://dev.azure.com/PlayFabPrivate/Switch/_git/PlayFabCSdk.Switch) |
| Legacy C++                        | [Android, iOS, Linux, Windows](playfab-cpp/index.md), [Switch](https://dev.azure.com/PlayFabPrivate/Switch/_git/XPlatCppSdk-Private-Switch), [PlayStation 4](https://dev.azure.com/PlayFabPrivate/PS4/_git/XPlatCppSdk-Private-Ps4), [PlayStation 5](https://dev.azure.com/PlayFabPrivate/PS5/_git/XPlatCppSdk-Private-PS5) |
| C#                                | [Xamarin](c-sharp/index.md) and other C#/.NET environments besides Unity |
| Java                              | [Android apps](java/index.md) |
| JavaScript                        | [Web Development](javascript/index.md) |
| Lua (community supported)         | [Corona (now Solar2D), Defold](lua/index.md) |
| NodeJS                            | [Node.js applications](nodejs/index.md)|
| Objective-C (community supported) | [iOS](objective-c/index.md)|
| Python (community supported)      | [Python](python/index.md)|

## By platform/operating system

| Platform/operating system | SDK/library                       |
|---------------------------|-----------------------------------|
| Android                   | [C# (using Xamarin)](c-sharp/index.md), [Java/Android Studio](java/index.md), [Lua](lua/index.md) (community supported), [Unity](unity3d/index.md), [Unreal Engine](unreal/index.md) |
| iOS                       | [C# (using Xamarin)](c-sharp/index.md), [Lua](lua/index.md) (community supported), [Objective-C](objective-c/index.md) (community supported), [Unity](unity3d/index.md), [Unreal Engine](unreal/index.md) |
| Linux                     | [Legacy C++](playfab-cpp/index.md), [Lua](lua/index.md) (community supported)|
| GDK (Xbox and Windows)    | [C/C++](c/index.md), [Unity](unity3d/index.md), [Unreal Engine](unreal/index.md) |
| PlayStation 4             | [Legacy C++](https://dev.azure.com/PlayFabPrivate/PS4/_git/XPlatCppSdk-Private-Ps4), [Unity](unity3d/index.md), [Unreal Engine](unreal/index.md) |
| PlayStation 5             | [Legacy C++](https://dev.azure.com/PlayFabPrivate/PS5/_git/XPlatCppSdk-Private-PS5), [Unity](unity3d/index.md), [Unreal Engine](unreal/index.md) |
| Switch                    | [C/C++](https://dev.azure.com/PlayFabPrivate/Switch/_git/PlayFabCSdk.Switch), [Legacy C++](https://dev.azure.com/PlayFabPrivate/Switch/_git/XPlatCppSdk-Private-Switch), [Unity](unity3d/index.md), [Unreal Engine](unreal/index.md)               |
| Windows (Win32)           | [C/C++](c/index.md), [Legacy C++](playfab-cpp/index.md), [Lua](lua/index.md) (community supported), [Unity](unity3d/index.md), [Unreal Engine](unreal/index.md) |
| Services and Tools        | [C#](c-sharp/index.md), [Java](java/index.md), [JavaScript](javascript/index.md), [Node.js](nodejs/index.md), [Python](python/index.md)

## By game engine

| Game engine               | SDK/library                       |
|---------------------------|-----------------------------------|
| Cocos2D                   | [Cocos2D](cocos2d-x/index.md) (community supported) |
| Unity                     | [Unity SDK](unity3d/index.md)|
| Unreal Engine             | [Unreal SDK](unreal/index.md)|

## See also

* [SDKs overview](sdk-overview.md)
* [What is PlayFab?](../what-is-playfab.md)
