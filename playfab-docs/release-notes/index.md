---
title: PlayFab Services SDK Release Notes 2023
author: amccalib
description: PlayFab Services SDK Release Notes for 2023.
ms.author: andmcc
ms.date: 07/10/2023
ms.topic: article
ms.service: playfab
keywords: playfab, development, release, apis, features
ms.localizationpriority: medium
---
# PlayFab Services SDK Release Notes 2023

> [!NOTE]
> For release notes about service releases and product updates, see the [release notes](https://github.com/PlayFab/PlayFab/releases) section on [PlayFab's public GitHub repository](https://github.com/PlayFab/PlayFab)

## 231013

Date: October 13, 2023

- Added IgnoreNonce and IssuerOverride to Create and Update OpenIdConnection requests in the Admin API
- Added SwedenCentral to AzureRegion in the Multiplayer API

## 230929

Date: September 29, 2023

 - Added Actions array to support getting and setting actions for scheduled tasks
 - Added models for all scheduled task action types
 - Added RequestPartyService call to the Multiplayer API
 - Added new error code for InvalidStatisticScore
 - Added new error codes for Lobby scenarios:
   - LobbyAssociatedServerMismatch
   - LobbyAssociatedServerNotFound
   - LobbyAssociatedToDifferentServer
   - LobbyServerAlreadyAssociated
   - LobbyIsNotClientOwned
   - LobbyDoesNotUseConnections

## 230915

Date: September 15, 2023

 - Added PageSize and SkipToken to ListContainerImageTagsRequest and Response in the Multiplayer API
 - Added AttributeStatistics and Scores properties to the Statistics field of Profile objects returned in the Profile API
 - Added LinkNintendoServiceAccountSubject call to the Server API

## 230901

Date: September 1, 2023

 - Added new Admin API call: DeleteMasterPlayerEventData
 - Added new error code for LeaderboardColumnLengthMismatch
 - Added OperationStatus to TransferInventoryItemsResponse in the Economy API

## 230818

Date: August 18, 2023

 - Added multiple error codes related to Managed Events:
   - ManageEventNamespaceInvalid
   - ManageEventNameInvalid
   - ManagedEventNotFound
   - ManageEventsInvalidRatio
   - ManagedEventInvalid
 - Added ServerCustomIdInfo to UserAccountInfo
 - Added "Unknown" to ContinentCode and CountryCode

## 230804

Date: August 4, 2023

- Minor reference documentation updates across multiple APIs

## 230721

Date: July 21, 2023

- Updated reference documentation for Economy V1 calls

## 230707

Date: July 7, 2023

- Added TelemetryKey management to Events API
- Removed LeaderboardMetadata from EntityProfile in GetEntity calls - this value was unused so no risk of a breaking change
- Added LinkPSNId to Server API

## 230623

Date: June 23, 2023

- Added error codes related to Addon management
- Added Language to SearchItemsRequest in the Economy API
- Added support for TelemetryKey auth to the Unity SDK
- Added Support for Unreal Engine 5.2

## 230609

Date: June 9, 2023

- Added error code for PartySerializationError
- Added TicketIsServiceSpecific to LoginWithSteam in the Client API
- Added UnitAmount to CatalogPrice in the Economy API
- Added support for TelemetryKey auth to the Unreal, XplatCpp, and C# SDKs

## 230529

Date: May 29, 2023

- Added Dadsv5 as a valid AzureVmFamily along with related AzureVmSize choices to the Multiplayer API
- Added PublicIPV4Addresses to GetMultiplayerServerDetails response in the Multiplayer API

## 230512

Date: May 12, 2023

- Added error code for TelemetryKeyLongInsightsRetentionNotAllowed
- Added support for a macOS build target to XplatCpp SDK

## 230428

Date: April 28, 2023

- Added multiple error codes related to PlayerCustomProperties:
    - PlayerCustomPropertiesPropertyNameTooLong
    - PlayerCustomPropertiesPropertyNameIsInvalid
    - PlayerCustomPropertiesStringPropertyValueTooLong
    - PlayerCustomPropertiesValueIsInvalidType
    - PlayerCustomPropertiesVersionMismatch
    - PlayerCustomPropertiesPropertyCountTooHigh
    - PlayerCustomPropertiesDuplicatePropertyName
    - PlayerCustomPropertiesPropertyDoesNotExist
- Added VmStartupScriptConfiguration to GetBuild response in the Multiplayer API

## 230403

Date: April 3, 2023

- Removed GetServerBuildUploadUrl, a legacy server hosting call, in the Admin API
- Added error code for AnalyticsSegmentCountOverLimit
- Added DurationInSeconds to AddInventoryItemsOperation in the Economy API
- Added RedirectUri to RedeemPlayStationStoreInventoryItems in the Economy API
- Added GetTitlePlayersFromXboxLiveIDs to the Profiles API
- Added LinkSteamId and UnlinkSteamId to the Server API

## 230320

Date: March 20, 2023

- Supports the [March 13 2023 PlayFab service release](https://github.com/PlayFab/PlayFab/releases/tag/untagged-ee9d08281cf8b7b22c9c)
- Added error code for TelemetryKeyDeactivated
- Removed the following calls related to legacy server hosting from various APIs:
    - Admin/GetMatchmakerGameInfo
    - Admin/GetMatchmakerGameModes
    - Admin/ModifyServerBuild
    - Client/GetCurrentGames
    - Client/GetGameServerRegions
    - Client/Matchmake
    - Matchmaker/AuthUser
    - Matchmaker/PlayerJoined
    - Matchmaker/PlayerLeft
    - Matchmaker/UserInfo
    - Server/DeregisterGame
    - Server/NotifyMatchmakerPlayerLeft
    - Server/RedeemMatchmakerTicket
    - Server/RefreshGameServerInstanceHeartbeat
    - Server/RegisterGame
    - Server/SetGameServerInstanceData
    - Server/SetGameServerInstanceState
    - Server/SetGameServerInstanceTags
- Removed Region from RefundPurchaseResponse in the Admin API
- Removed UseStreamingForAssetDownloads from multiple calls in the Multiplayer API

## 230306

Date: March 6, 2023

- Added error codes for these errors:
    - EntityAPIKeysNotSupported
    - IpAddressBanned
    - EntityLineageBanned
    - NamespaceMismatch
    - InvalidServiceConfiguration
    - InvalidNamespaceMismatch
    - TelemetryKeyNotFound
    - TelemetryKeyInvalidName
    - TelemetryKeyAlreadyExists
    - TelemetryKeyInvalid
    - TelemetryKeyCountOverLimit
- Added SetEmail to LoginWithGoogleAccountRequest in the Client API
- Made the following addition to the Economy API:
    - Added DurationInSeconds to multiple item-related request and operations
    - Added UnitDurationInSeconds to CatalogPrice
    - Added DefaultStackId to CatalogIte
    - Added ExpirationDate to InventoryItem

## 230220

Date: February 20, 2023

- Added error code for InvalidNintendoSwitchAccountId
- Added VmStartupScriptConfiguration to multiple calls in the Multiplayer API

## 230206

Date: February 6, 2023

- Added error codes for these errors:
    - AnalysisSubscriptionNotFound
    - AnalysisSubscriptionFailed
    - AnalysisSubscriptionFoundAlready
    - AnalysisSubscriptionManagementInvalidInput
    - InvalidGameCenterId
- Removed Amount as a required value on multiple calls in the Economy API

## 230123

Date: January 23, 2023

- Fixed memory leak in Unity Editor Extensions
- Added support for sending unsent events on shutdown to the XplatCpp SDK

## 230109

Date: January 9, 2023

- Fixed bug in ValidateEntityToken in the C# SDK