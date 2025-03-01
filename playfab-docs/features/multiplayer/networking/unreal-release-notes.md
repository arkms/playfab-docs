---
title: PlayFab OnlineSubsystem for Unreal Engine 4 and 5 Release Notes
author: PushpadantK
description: Release notes for PlayFab OnlineSubsystem for Unreal Engine 4 and 5
ms.author: pkacha
ms.date: 11/29/2021
ms.topic: article
ms.service: playfab
keywords: playfab, party, unreal, release notes, multiplayer, networking
ms.localizationpriority: medium
---

# PlayFab Unreal Engine OnlineSubsystem release notes
Refer to [QuickStart: PlayFab Online Subsystem (OSS)](party-unreal-engine-oss-quickstart.md) for download and install instructions.
## 2.3.0
- Supported UE5.2 and previous UE versions (UE4.27+, UE5.0, and UE5.1. Refer to [QuickStart: Which versions of Unreal Engine are supported](party-unreal-engine-oss-overview.md#which-versions-of-unreal-engine-are-supported)).

Feature fixes:
- Implemented `FOnlineSessionPlayFab::SendSessionInviteToFriends` and `FOnlineExternalUIPlayFab::ShowInviteUI` for GDK, Steam, and PlayStation with native platform invites
- Fixed the display of player platform ID
- Fixed failure to update member properties and lobby search keys
- Fixed failure to play new game after suspend and resume on the Xbox platform
- Fixed microphone audio issue on GDK
- Fixed the modification on `bIsDedicated` in `OnlineSessionInterfacePlayFab`

Compile fixes:
- Deprecated XboxOne and replaced it with XB1 for Unreal Engine 5.2
- Resolved build warnings, non-unity build errors, compilation issues when users lack access to Unreal Engine across all platforms

Known issue:
- To invite a Steam or PlayStation player, the host must be on the same platform.

## 2.0.0
- UE4 engine OSS PlayFab is updated to use Multiplayer features offered by Azure PlayFab such as Lobby, Matchmaking along with PlayFab Party.
This replaces the Xbox provided MPSD with Azure PlayFab Lobby and XBL Smart match with Azure Matchmaking service.
- XDK is not longer supported for this version of the OSS

## 1.0.7
UE4 Engine version 4.26 is the recommended version to use with this version of OnlineSubsystemPlayfab.
### Notes:
Rename OnlineSubsystemPlayFabParty to OnlineSubsystemPlayfab.



