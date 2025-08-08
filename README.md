<h1 align="center">Rendering API</h1>

### Metal
###### MacOS Only
```json
{
    "FFlagDebugGraphicsPreferMetal": "True"
}
```
### Vulkan
```json
{
    "FFlagDebugGraphicsDisableDirect3D11": "True",
    "FFlagDebugGraphicsPreferVulkan": "True"
}
```
### OpenGL
```json
{
    "FFlagDebugGraphicsDisableDirect3D11": "True",
    "FFlagDebugGraphicsPreferOpenGL": "True"
}
```
### Direct X 10
```json
{
    "FFlagDebugGraphicsPreferD3D11FL10": "True"
}
```
### Direct X 11
```json
{
    "FFlagDebugGraphicsPreferD3D11": "True"
}
```

<h1 align="center">Lightning Technologies</h1>

### Voxel Lighting (Phase 1)
```json
{
    "DFFlagDebugRenderForceTechnologyVoxel": "True"
}
```
### Shadowmap Lighting (Phase 2)
```json
{
    "FFlagDebugForceFutureIsBrightPhase2": "True"
}
```
### Future Lighting (Phase 3)
```json
{
    "FFlagDebugForceFutureIsBrightPhase3": "True"
}
```
### Unified lighting
```json
{
    "FFlagRenderUnifiedLighting16": "True"
}
```
### Unified Lighting Blendzone
```json
{
    "FIntUnifiedLightingBlendZone": "500"
}
```

<h1 align="center">Graphical Settings</h1>

### Disble DRS
```json
{
    "FFlagRenderDynamicResolutionScale12": "False"
}
```

### disable highlights
###### stops highlights from showing on parts
###### @satlybpro
```json
{
    "DFFlagRenderHighlightManagerPrepare": "True"
}
```
### Makes stuff slightly brighter
```json
{
    "FFlagRenderFixFog": "True"
}
```
### HyperThreading
```json
{
    "FFlagDebugCheckRenderThreading": "True",
    "FFlagRenderDebugCheckThreading2": "True"
}
```
### Maximum Threads
```json
{
    "FIntRuntimeMaxNumOfThreads": "2400"
}
```
### Minimum Threads
```json
{
    "FIntTaskSchedulerThreadMin": "3"
}
```
### Smoother Terrain
```json
{
    "FFlagDebugRenderingSetDeterministic": "True"
}
```
### Force Graphics Quality Level
```json
{
    "FIntRomarkStartWithGraphicQualityLevel": "1"
}
```
### Disable Player Shadows
```json
{
    "FIntRenderShadowIntensity": "0"
}
```
### Preserve rendering quality with display setting
```json
{
    "DFFlagDisableDPIScale": "True"
}
```
### Low Graphics Quality w/ Max Render Distance/FRM Quality Levels
###### Explanation: 1-6 Are low graphics, Above 6 are high graphics.
```json
{
    "DFIntDebugFRMQualityLevelOverride": "1"
}
```
<h4 align="center">FRM Levels</h4>

```
Low

1 = 3
2 = 2
3 = 6

High

4 = 7
5 = 11
6 = 14
7 = 15 
8 = 17
9 = 18
10 = 21
```
### Low Render Distance
```json
{
    "DFIntDebugRestrictGCDistance": "1"
}
```
### Pixelated graphics
###### This flag makes your graphics pixelated, higher values will show you more pixels
```json
{
    "DFIntDebugDynamicRenderKiloPixels": "1"
}
```
### Limits light updates
```json
{
    "FIntRenderLocalLightUpdatesMax": "8",
    "FIntRenderLocalLightUpdatesMin": "6"
}
```
### Disables fade in and fade out animation every light update
```json
{
    "FIntRenderLocalLightFadeInMs": "0"
}
```
### Makes avatars shiny 
###### [everything goes black on <3] ***[DFIntDebugFRMQualityLevelOverride is there to set your graphics to 10, You can change it to anything above 3***
```json
{
    "DFIntRenderClampRoughnessMax": "-640000000",
    "DFIntDebugFRMQualityLevelOverride": "6"
}
```
### Disable PostFX
```json
{
    "FFlagDisablePostFx": "True"
}
```
### Pause Voxelizer/Disable Baked Shadows
```json
{
    "DFFlagDebugPauseVoxelizer": "True"
}
```
### Gray Sky
###### Only applies to games with the default skybox
```json
{
    "FFlagDebugSkyGray": "True"
}
```
### White Sky
###### Only applies to games with the default skybox
```json
{
    "FFlagDebugSkyGray": "True",
    "FFlagSkyUseRGBEEncoding": "True"
}
```
### Force LOD on Meshes
```json
{
    "DFIntCSGLevelOfDetailSwitchingDistance": "0",
    "DFIntCSGLevelOfDetailSwitchingDistanceL12": "0",
    "DFIntCSGLevelOfDetailSwitchingDistanceL23": "0",
    "DFIntCSGLevelOfDetailSwitchingDistanceL34": "0"
}
```
### Lighting Attenuation
```json
{
    "FFlagNewLightAttenuation": "True"
}
```
### Enable GPULightCulling
###### Combine with [Lighting Attenuation](https://github.com/d44df016fe28bc8d5974/rbxflags#lighting-attenuation) for better vision
```json
{
    "FFlagFastGPULightCulling3": "True"
}
```
### Enable CPULightCulling
```json
{
    "FFlagDebugForceFSMCPULightCulling": "True"
}
```
### Frame Buffer
###### Explanation: 0 makes white screen 1-3 makes other players have laggy movement, 4 is stable has better performance than 10 and less input lag
```json
{
    "DFIntMaxFrameBufferSize": "4"
}
```
### Average Frame Delay
```json
{
    "DFIntMaxAverageFrameDelayExceedFactor": "3"
}
```
### Average Frame Delay + Frame Buffer
```json
{
    "DFIntMaxFrameBufferSize": "1",
    "FIntInterpolationAwareTargetTimeLerpHundredth": "100",
    "DFIntMaxAverageFrameDelayExceedFactor": "0"
}
```
### Low Quallity Terrain Textures
###### 4 for less quality 16, 32, 64 for higher quality
```json
{
    "FIntTerrainArraySliceSize": "4"
}
```
### High Quality Textures 
###### *[1-3]*
```json
{
    "DFFlagTextureQualityOverrideEnabled": "True",
    "DFIntTextureQualityOverride": "3"
}
```
### Lower Quality Textures 
###### *[1-3]*
```json
{
    "DFIntPerformanceControlTextureQualityBestUtility": "-1"
}
```
### No avatar textures
```json
{
    "DFIntTextureCompositorActiveJobs": "0"
}
```
### Texture Manager
###### 1-4 Blurry, 5-7 low quality also removes studs, 8 Removes almost everything
```json
{
    "FIntDebugTextureManagerSkipMips": "8"
}
```
### Remove Grass
```json
{
    "FIntFRMMinGrassDistance": "0",
    "FIntFRMMaxGrassDistance": "0",
    "FIntRenderGrassDetailStrands": "0"
}
```
### Increased Grass Motion
###### really fast speed
###### @spectro
```json
{
    "FIntGrassMovementReducedMotionFactor": "999"
}
```
### No Grass Motion
###### @spectro
```json
{
    "FIntGrassMovementReducedMotionFactor": "0"
}
```
### Enable Highlight Outlines on any Rendering API
```json
{
    "FFlagHighlightOutlinesOnMobile": "True"
}
```
### Force MSAA 
###### *[0, 1, 2, 4, 8]*
```json
{
    "FIntDebugForceMSAASamples": "4"
}
```
### ShadowMap Bias 
###### ***[Future & ShadowMap]***
```json
{
    "FIntRenderShadowmapBias": "75"
}
```
### Limits number of animations being played
###### 0 removes most player animations, 1-5 removes the walk animation after jumping
```json
{
    "DFIntMaxActiveAnimationTracks": "0"
}
```
### Increased Particles on low graphics
###### @teeenoob
```json
{
    "FFlagDebugDeterministicParticles" : "True"
}
```
### No clouds/Sky
###### @Bloxy,@5070
```json
{
    "FFlagRenderNoLowFrmBloom": "false",
    "FFlagFRMRefactor": "false"
}
```
<h1 align="center">Quality of Life</h1>

### Disable Captures Keybind
```json
{
    "FFlagEnableCapturesHotkeyExperiment_v4": "False"
}
```
### Unlimited FPS Unlocker
```json
{
    "FFlagTaskSchedulerLimitTargetFpsTo2402": "False",
    "FFlagGameBasicSettingsFramerateCap5": "False",
    "DFIntTaskSchedulerTargetFps": "9999"
}
```
### GUI Hiding Toggles
```json
{
    "FFlagUserShowGuiHideToggles": "True",
    "GuiHidingApiSupport2": "True"
}
```
### Hide guis
###### ***Instructions: Replace "ID" with any group ID that you are in.***
| Key combination   | Action                                                                    |
| ----------------- | ------------------------------------------------------------------------- |
| Ctrl + Shift + B  | Toggles GUIs in 3D space (BillboardGuis, SurfaceGuis, etc)                |
| Ctrl + Shift + C  | Toggles game-defined ScreenGuis                                           |
| Ctrl + Shift + G  | Toggles Roblox CoreGuis                                                   |
| Ctrl + Shift + N  | Toggles player names, and other BillboardGuis that show up above a player |
```json
{
    "DFIntCanHideGuiGroupId": "ID"
}
```
### Remove layered clothing related for searching in lua app catalog
###### From: https://discord.gg/nKjV3mGq6R
```json
{
    "FStringAXCategories": "ClassicShirts.ClassicTShirts.ClassicPants"
}
```
### Disable Fullscreen Title Bar
```json
{
    "FIntFullscreenTitleBarTriggerDelayMillis": "3600000"
}
```
### Disable In-game Advertisements
```json
{
    "FFlagAdServiceEnabled": "False"
}
```
### Spammed letters
###### This fflag basically spams every other letter on roblox coregui and the game's gui but it doesn't affect some parts of the games.
###### Default is 0 and if you set it to anything higher it just follows whatever number you put
```json
{
    "FIntDebugTextElongationFactor": "999999"
}
```
### Surf the web inside of Roblox
###### Click the Beta badge or the 13+ badge to open the webview browser.
```json
{
    "FFlagTopBarUseNewBadge": "True",
    "FStringTopBarBadgeLearnMoreLink": "https://google.com/",
    "FStringVoiceBetaBadgeLearnMoreLink": "https://google.com/"
}
```
### MTU 
```json
{
    "DFIntConnectionMTUSize": "MTU_HERE"
}
```
### Adjust Default Timeout Time
###### 1 second = 1000
###### @dis_spencer
```json
{
    "DFIntDefaultTimeoutTimeMs": "10000"
}
```
### Quick Game Launch 
###### *[BUGGY]*
```json
{
    "FFlagEnableQuickGameLaunch": "True"
}
```
### Disable In-Game Purchases
```json
{
    "DFFlagOrder66": "True"
}
```
### Disable Chat
```json
{
    "FFlagDebugForceChatDisabled": "True"
}
```
### Disable Dynamic Heads Animations
###### https://roblox.fandom.com/wiki/Dynamic_Head
```json
{
    "DFIntAnimationLodFacsDistanceMin": "0",
    "DFIntAnimationLodFacsDistanceMax": "0",
    "DFIntAnimationLodFacsVisibilityDenominator": "0"
}
```
### Automatically unmutes your mic on join (VC)
```json
{
    "FFlagDebugDefaultChannelStartMuted": "False"
}
```
### opt-out Experience Language
###### Removes the Experience Language option in settings
```json
{
    "FIntV1MenuLanguageSelectionFeaturePerMillageRollout": "0"
}
```
### Lets you change the zoom out limit
###### Only applies to games that haven't changed the default zoom limit
```json
{
    "FIntCameraMaxZoomDistance": "9999"
}
```
### Exclusive Fullscreen
```json
{
    "FFlagHandleAltEnterFullscreenManually": "False"
}
```
### Changes some tiny things about Party
```json
{
    "FFlagAppChatAddConnectUnibarForActiveSquad": "False"
}
```
### Reshuffle Party Icons
###### Changes the position of the "in a party" icon in the top bar
```json
{
    "FFlagReshufflePartyIconsInUnibar": "False"
}
```
### Renames Party back to Roblox Chat
```json
{
    "FFlagAppChatRebrandStringUpdates": "False"
}
```
### Disable reduced avatar item particles in first person
###### disables reducing particle effect transparency if you go to first person
```json
{
    "FFlagUserHideCharacterParticlesInFirstPerson": "False"
}
```
### Increased preloading asset count
###### Load into games faster
```json
{
    "DFIntNumAssetsMaxToPreload": "9999999",
    "DFIntAssetPreloading": "9999999"
}
```
### 5 decimal digits limit for camera sensitivity
###### basically like idk 8 months ago roblox added a 3 decimal digits limit, some people that I know used those extra digits
```json
{
    "FFlagFixSensitivityTextPrecision": "False"
}
```
### Disable voicechat
###### Setting this to True will not do anything 
###### [TIP] Use PlaceFilter for specific games
```json
{
    "DFFlagVoiceChat4": "False"
}
```
<h1 align="center">User Interface/Visuals</h1>

### V2 Menu
###### enables the 2020 sidebar menu
```json
{
    "FIntNewInGameMenuPercentRollout3": "100",
    "FFlagEnableInGameMenuControls": "False",
    "FFlagDisableNewIGMinDUA": "True",
    "FFlagEnableInGameMenuChromeABTest4": "False",
    "FFlagEnableInGameMenuChrome": "false",
    "FFlagEnableInGameMenuSongbirdABTest": "False"
}
```
### Custom Disconnect Message
```json
{
    "FFlagReconnectDisabled": "True",
    "FStringReconnectDisabledReason": "You're stupid and I hate you"
}
```
### Display FPS
```json
{
    "FFlagDebugDisplayFPS": "True"
}
```
### Verified Badge
###### clientsided, only you can see the badge
```json
{
    "FStringWhitelistVerifiedUserId": "UserID"
}
```
### Verified Badge on everyone
###### clientsided, only you can see the badge
```json
{
    "FFlagOverridePlayerVerifiedBadge": "True"
}
```
###  Neon Rainbow Guis
```json
{
    "FFlagDebugDisplayUnthemedInstances": "True"
}
```
### Remove Disconnect Blur/Loading Blur
```json
{
    "FIntRobloxGuiBlurIntensity": "0"
}
```
### Disable New Chat Translation Settings
```json
{
    "FFlagChatTranslationSettingEnabled3": "False"
}
```
### New Camera Mode
```json
{
    "FFlagNewCameraControls": "True"
}
```
### Custom MicroProfiler Scale
```json
{
    "DFIntMicroProfilerDpiScaleOverride":  "100"
}
```
### Set Custom Font Size
```json
{
    "FIntFontSizePadding": "1"
}
```
### red font
###### You need to use Default Roblox Font to activate this. Also it can be glitchy in the settings menu
```json
{
    "FStringDebugHighlightSpecificFont": "rbxasset://fonts/families/BuilderSans.json"
}
```
### New Report Menu
```json
{
    "FStringSelectInSceneReportMenuOverrideUserIds": "UserID"
}
```
### Always display Render Stats
###### pretty self explanatory fflag, you can't disable them using the hotkey
```json
{
    "FFlagDebugAlwaysDisplayRenderStats": "true"
}
```
### Adjust Scroll Speed
```json
{
    "FIntScrollWheelDeltaAmount": "140"
}
```
### Set Custom Kick Message Length
```json
{
    "FIntMaxKickMessageLength": "1"
}
```
### Darker Dark Theme
```json
{
    "FFlagLuaAppUseUIBloxColorPalettes1": "True",
    "FFlagUIBloxUseNewThemeColorPalettes": "True"
}
```
### Enable New Settings Layout
```
{
    "FFlagInExperienceMenuReorderFirstVariant2": "True"
}
```
### Reset Character instead of Respawn in Experience Menu
```json
{
    "FFlagInExperienceMenuResetButtonTextToRespawn": "False"
}
```
### No Transparency V4 Menu **(2023)**
```json
{
    "FStringInGameMenuModernizationStickyBarForcedUserIds": "UserID"
}
```
### Subscriptions Page
```json
{
    "FFlagLuaAppDevSubsEnabled": "True"
}
```
### Overlay that shows what you type 
```json
{
    "FFlagDebugTextBoxServiceShowOverlay": "True"
}
```
### Ammount of lines to show at once for above
```json
{
    "DFIntTextBoxServiceHistorySize": "1"
}
```
### Hides gui
```json
{
    "FFlagDebugAdornsDisabled":  "True"
}
```
### disable coregui
###### you get a white screen if you use the lua app and all coreguis dont show up if you're ingame
###### @satlybpro
```json
{
    "FFlagFFlagLogAllGuacRead":  "True"
}
```
### Dont Render UI
```json
{
    "FFlagDebugDontRenderUI": "True"
}
```
### Dont Render Screen GUIs
```json
{
    "FFlagDebugDontRenderScreenGui": "True"
}
```
### Break Top Bar Menu
```json
{
    "FStringNewInGameMenuForceds": "UserID",
    "FFlagEnableInGameMenuChrome": "True"
}
```
### Break Collectible Icon
```json
{
    "FFlagDisplayCollectiblesIcon": "False"
}
```
### Disable Bubble Chat
```json
{
    "FFlagEnableBubbleChatFromChatService": "False"
}
```
### Disable Camera & Selfview
```json
{
    "FFlagSelfieViewEnabled": "True"
}
```
### Disable Avatar Chat
```json
{
    "FFlagAvatarChatServiceEnabled3": "False"
}
```
### Remove VC Beta Badge
```json
{
    "FFlagVoiceBetaBadge": "False",
    "FFlagTopBarUseNewBadge": "False",
    "FFlagBetaBadgeLearnMoreLinkFormview": "False",
    "FFlagControlBetaBadgeWithGuac": "False",
    "FStringVoiceBetaBadgeLearnMoreLink": "null"
}
```
### VR Controller transparency
```json
{
    "FIntVRTouchControllerTransparency": "0"
}
```
### Disable VR Collision Fade
###### @Sky
```json
{
    "FFlagViewCollisionFadeToBlackInVR": "False"
}
```
### Limit Videos Playing
```json
{
    "DFIntVideoMaxNumberOfVideosPlaying": "0"
}
```
### Disable DSA Reporting In-game
```json
{
    "FFlagDSAIllegalContentReporting2": "False"
}
```
### Desktop App Dev Tools
###### only works on web view windows like profiles, ctrl + shift + I
```json
{
    "FFlagDebugEnableNewWebView2DevTool": "True"
}
```
### Show All Error Strings
###### makes you unable to join games and shows you every join error message
```json
{
    "FFlagDebugEnableErrorStringTesting": "True"
}
```
### Customize chat translation settings
###### A fflag that lets you customize what languages are available for the chat translation feature
###### (English cannot be removed)
###### @thefrenchguy4
```json
{
    "FStringChatTranslationEnabledLocales": "es_es,fr_fr,pt_br,de_de,it_it,ja_jp,ko_kr,id_id,tr_tr,zh_cn,zh_tw,th_th,pl_pl,vi_vn,ru_ru,"
}
```
### Remove the "automatically translation" message
###### basically remove that message when you join a game that roblox will automatically translate supported languages etc etc
###### @toofastforboo
```json
{
    "FFlagChatTranslationEnableSystemMessage": "False"
}
```
### remove the vr toggle
###### removes the vr toggle from the escape menu
```json
{
    "FFlagAlwaysShowVRToggleV3": "False"
}
```
### cleaner desktop home page
###### Tho it wont remove the Recommended for you and Sponsored sections but it will remove the Recommended section (the insanely long one)
```json
{
    "FIntGameGridFlexFeedItemTileNumPerFeed": "0"
}
```
### disable burger icon
###### removes the 2015 3 lines icon from chrome ui and reverts it to the 9 dots square
```json
{
    "FFlagEnableHamburgerIcon": "False"
}
```
### Old chrome ui chat icon
```json
{
    "FFlagAppChatRebrandIconUpdates": "False"
}
```
### Revert the new chrome ui to the old one
```json
{
    "FFlagEnableHamburgerIcon": "False",
    "FFlagEnableUnibarV4IA": "False",
    "FFlagEnableAlwaysOpenUnibar2": "False",
    "FFlagUseNewUnibarIcon": "False",
    "FFlagUseSelfieViewFlatIcon": "False",
    "FFlagUnibarRespawn": "False",
    "FFlagEnableChromePinIntegrations2": "False",
    "FFlagAppChatInExperienceEnabledV647new": "False"
}
```
### Extra + left healthbar for chrome ui Topbar
```json
{
    "FFlagEnableUnibarMaxDefaultOpen": "True",
    "FFlagUpdateHealthBar": "False",
    "FFlagUseNewPinIcon": "False"
}
```
### Fix broken health bar
```json
{
    "FFlagEnableAlwaysOpenUnibar2": "False"
}
```
### Roblox events button
###### remove FStringPlatformEventUrl to have the default url
```json
{
    "FFlagPlatformEventEnabled2": "True",
    "FStringPlatformEventUrl": "AnyLinkHere"
}
```
### Better Trackpad Scrolling
```json
{
    "FFlagBetterTrackpadScrolling": "True"
}
```
### Reset Character instead of Respawn in Experience Menu
```json
{
    "FFlagInExperienceMenuResetButtonTextToRespawn": "False"
}
```
### Mini webview
```json
{
    "FFlagWebViewProtocol": "False"
}
```
### Google guidelines
###### Makes the Learn More button in the Age rating button redirect to the link of your choice
###### desktop app only
```json
{
    "FStringExperienceGuidelinesExplainedPageUrl": "url"
}
```
### No opacity to Chrome UI
###### So when this fflag is set to false when you change the background transparency in the esc menu it won't affect the small 3 buttons of chrome ui and will keep them semi-transparent
###### the bg transparency set to opaque and the fflag is true and one on the right is bg transparency set to opaque and the fflag is false
###### @satlybpro
```json
{
    "FFlagChromeUsePreferredTransparency": "False"
}
```
### Preferred text size scale
###### enables a font scaler in the escape menu
###### @Sky
```json
{
     "FFlagEnablePreferredTextSizeScale": "True",
     "FFlagEnablePreferredTextSizeSettingInMenus2": "True"
}
```
### Explorer Redesign
###### studio only
###### @easternbloxxer
```json
{
    "FFlagExplorerPropertiesUseRDLColors": "True",
    "FFlagExplorerPropertiesUseStyledObject": "True"
}
```
### Mute button redesign (VC)
###### changes the vc mute button in the menu
```json
{
    "FFlagMuteTogglesEnableIXP": "False"
}
```
### Multi Try On
###### Allows you to try on multiple things in the catalog and buy everything at once
###### some accessories in the same category cannot be tried on at the same time
```json
{
   "FFlagAXEnableMultiTryOnUI": "True"
}
```
<h1 align="center">User Interface/Visuals Experimental</h1>

### Simple coregui settings
```
{
    "FFlagRefactorInExpGameSettings": "True"
}
```
### Capture posts
###### twitter but roblox edition
```
{
    "FFlagCapturesPostEnabledForAll_v4": "true"
}
```
### Enable Better Haptics
```json
{
    "FFlagEnableBetterHapticsResultHandling": "True"
}
```
### Hide playerlist close button on Chrome UI
```json
{
    "FFlagDisablePlayerListDisplayCloseBtn": "True"
}
```
### Ragdoll Death Type
#### Studio Only
###### I tried `Ragdoll` to see if anything would happen lol this is how i found this (found this long time ago)
```json
{
    "DFStringDefaultAvatarDeathType": "Ragdoll"
}
```
<h1 align="center">Audio Related</h1>

### Allows you to change voice chat distance 
###### default: [Min 7 Max 80]
```json
{
    "DFIntVoiceChatRollOffMinDistance": "7",
    "DFIntVoiceChatRollOffMaxDistance": "80"
}
```
### Sounds use physical velocity and become distorted
###### <2017
```json
{
    "FFlagSoundsUsePhysicalVelocity": "True"
}
```
### Audio Occlusion
```json
{
    "FFlagDebugEnableDirectAudioOcclusion2": "True"
}
```
### Limit audios that are being played
```json
{
    "DFIntMaxLoadableAudioChannelCount": "1"
}
```
### Mess with voice chat volume
###### default 1000
```json
{
    "DFIntVoiceChatVolumeThousandths": "100000"
}
```
### No sounds
```json
{
    "FFlagDebugRomarkMockingAudioDevices": "True"
}
```

### Remove Parental Controls Tab
```json
{
    "FFlagLuaAppsEnableParentalControlsTab": "False"
}
```
### Legacy Search
```json
{
    "FFlagAXSearchLandingPageIXPEnabled4": "False"
}
```
### Disable Profile Picture Customization
```json
{
    "FFlagAXDefaultAvatarToShopEnabled3": "False"
}
```
### old luaapp chat button
```json
{
    "FStringNewChatTabExperimentLayerValue": "2024MUSIC"
}
```
### Disable Toast Notifications
```json
{
    "FFlagToastNotificationsProtocolEnabled2": "False"
}
```
### Rename Communications to Voice Enabled
```json
{
    "FFlagGameDetailsDecoupledCommunication": "False"
}
```
<h1 align="center">Physics (Abusive)</h1>

### Terrain fly
```json
{
    "DFIntBulletContactBreakOrthogonalThresholdPercent": "-2147483647",
    "DFIntBulletContactBreakOrthogonalThresholdActivatePercent": "2147483647",
    "DFIntBulletContactBreakThresholdPercent": "15000"
}
```
### Tool Desync
```json
{
    "DFIntSimBlockLargeLocalToolWeldManipulationsThreshold": "-1"
}
```
### Remap R6 to R15 Rigs/Weird Movement
```json
{
    "FFlagRemapAnimationR6ToR15Rig": "True"
}
```
### Weird Leg Movement
```json
{
    "DFFlagAnimatorPostProcessIK": "True"
}
```
### Drunk
```json
{
    "DFIntSimAdaptiveHumanoidPDControllerSubstepMultiplier": "-999999",
    "DFFlagSimHumanoidTimestepModelUpdate": "True"
}
```
### Spinning
```json
{
   "DFIntSimTimestepMultiplierDebounceCount": "-1100000",
   "DFIntSimAdaptiveHumanoidPDControllerSubstepMultiplier": "-999999"
}
```
### No Animations
###### **Stops the game from trying to replicate your animations in the server. You dont have animations in the server but you do for your client**
```json
{
    "DFIntReplicatorAnimationTrackLimitPerAnimator": "-1"
}
```
### Delayed Animations
###### your animations on your screen are normal but on the server they aren't
###### affects everyone's animations
###### @pyhlou
###### [video](https://streamable.com/68hru3)
```json
{
    "FFlagProcessAnimationLooped": "False"
}
```
### Stick unanchored parts to you
##### - = up, + = down
```json
{
    "DFIntSolidFloorPercentForceApplication": "-1000",
    "DFIntNonSolidFloorPercentForceApplication": "-5000"
}
```
### Max Raycast Distance
###### Raycasting is the use of intersection tests to solve problems in ROBLOX. The most common use of raycasting is to determine the first object intersected by a ray. This is done by casting a virtual ray from a certain point in a direction and determining the first surface it intersected with.
###### Break legs collision from 2 to -inf, kinda break camera on values over 3 noclip cam on 3
```json
{
    "DFIntRaycastMaxDistance": "3"
}
```
### Change DataSender Rate
###### a.k.a does not let you load games
```json
{
    "DFIntDataSenderRate": "-1"
}
```
### Disable Touch Events
```json
{
    "DFIntTouchSenderMaxBandwidthBps": "-1"
}
```
### Better serversided character position
###### 100 makes your serversided character closer to your client
```json
{
    "DFIntS2PhysicsSenderRate": "100"
}
```
### Invisible
###### Restricts the client from sending any physics-related information. This means other people can topple you over.
```json
{
    "DFIntPhysicsSenderMaxBandwidthBps": "1",
    "DFIntPhysicsSenderMaxBandwidthBpsScaling": "0"
}
```
### Clientsided Invisible
```json
{
    "FIntParallelDynamicPartsFastClusterBatchSize": "-1"
}
```
### Wallglide
```json
{
    "DFIntMaximumUnstickForceInGs": "-4"
}
```
### Ragdoll freeze
###### you freeze while you're ragdolled
```json
{
    "DFIntPhysicsImprovedCyclicExecutiveThrottleThresholdTenth": "0"
}
```
### less kb in sb
```json
{
    "DFIntPhysicsImprovedCyclicExecutiveThrottleThresholdTenth": "-1",
    "DFIntGameNetLocalSpaceMaxSendIndex": "100000"
}
```

### Slide on Terrain/Meshes
###### @tyetonix
```json
{
    "DFIntSmoothTerrainPhysicsRayAabbSlop": "-9999"
}
```
### Drive vehicles slowly
###### @tyetonix
```json
{
    "DFIntPhysicsImprovedCyclicExecutiveThrottleThresholdTenth": "0"
}
```
### Enhanced Wallhopping
###### @tyetonix
```json
{
    "DFIntMaximumFreefallMoveTimeInTenths": "9999999",
    "DFIntMinimumFreefallMoveDistanceInTenths": "100",
    "DFIntMaximumUnstickForceInGs": "-1",
    "DFIntUnstickForceDecayInTenths": "1",
    "DFIntUnstickForceEpsilonInHundredths": "1",
    "DFFlagFixFreefall": "true",
    "DFFlagFixFreefallCleanup": "true"
}
```
### Network Ownership
###### better [network ownership](https://create.roblox.com/docs/physics/network-ownership) of parts
```json
{
    "DFIntMinClientSimulationRadius": "2147000000",
    "DFIntMinimalSimRadiusBuffer": "2147000000",
    "DFIntMaxClientSimulationRadius": "2147000000",
    "DFFlagDebugPhysicsSenderDoesNotShrinkSimRadius": "True",
    "FFlagDebugUseCustomSimRadius": "True"
}
```
<h1 align="center">Abusive Visuals</h1>

### Semi Fullbright
```json
{
    "FFlagFastGPULightCulling3": "True",
    "FIntRenderShadowIntensity": "0",
    "DFIntCullFactorPixelThresholdShadowMapHighQuality": "2147483647",
    "DFIntCullFactorPixelThresholdShadowMapLowQuality": "2147483647",
    "FFlagNewLightAttenuation": "True",
    "FIntRenderShadowmapBias": "-1",
    "DFFlagDebugPauseVoxelizer": "True"
}
```
### Fullbright 1
###### use in games with massive or games with lots of clouds, make sure the game is daytime or has daytime.
###### @NoobLikesThis
```json
{
    "FFlagFastGPULightCulling3": "True",
    "FIntRenderShadowIntensity": "0",
    "DFIntCullFactorPixelThresholdShadowMapHighQuality": "2147483647",
    "DFIntCullFactorPixelThresholdShadowMapLowQuality": "2147483647",
    "FFlagNewLightAttenuation": "True",
    "FIntRenderShadowmapBias": "-1",
    "DFFlagDebugPauseVoxelizer": "True",
    "DFIntDebugFRMQualityLevelOverride": "1",
    "DFFlagDebugRenderForceTechnologyVoxel": "True",
    "FFlagRenderFixFog": "True",
    "FFlagDisablePostFx": "True"
}
```
### Fullbright 2
###### same stuff needed as fullbright but its better, fullbright 1 and 2 will let you noclip a bit inside a wall, be-aware.
###### tip: change the DFIntDebugFRMQualityLevelOverride fflag to 0 when you dont want quality 1 and wanna change it in game, best to hide ur fullbright while someone is watching.
###### @NoobLikesThis
```json
{
    "FFlagFastGPULightCulling3": "True",
    "FIntRenderShadowmapBias": "-1",
    "DFIntCullFactorPixelThresholdShadowMapHighQuality": "2147483647",
    "DFIntCullFactorPixelThresholdShadowMapLowQuality": "2147483647",
    "FIntRenderShadowIntensity": "0",
    "FFlagRenderFixFog": "True",
    "DFFlagDebugRenderForceTechnologyVoxel": "True",
    "FFlagRenderNoLowFrmBloom": "false",
    "DFIntDebugFRMQualityLevelOverride": "1",
    "FIntBloomFrmCutoff": "1654515",
    "DFFlagDebugPauseVoxelizer": "True",
    "FFlagNewLightAttenuation": "True",
    "FFlagFRMRefactor": "false",
    "FFlagDisablePostFx": "True"
}
```
### Humanoid Outline
##### Draws an outline around every part and every humanoid
```json
{
    "DFFlagDebugDrawBroadPhaseAABBs": "True"
}
```
### fflag above but more complex
##### Draws an outline around every body part
```json
{
    "DFFlagDebugDrawBvhNodes": "True"
}
```
### Buggy ZPlane Camera
###### setting this to 0 makes the map invisible
```json
{
    "FIntCameraFarZPlane": "1"
}
```
### Adds an UI in game, which highlights any part player touches (like ground, Meshes etc.). It's a non-functioning UI too. Also adds a blue circle to your humanoid.
```json
{
    "FFlagDebugHumanoidRendering": "True"
}
```

<h1 align="center">Abusive Game Specific Presets</h1>


<h1 align="center">lol</h1>

### omg i cant believe roblox is that dumb to do this...
> [!CAUTION]
> these fflags cause a memory leak + crashes roblox
```json
{
    "FIntPhysicsGridHierarchyLowestLevelInitBinCount": "199999999",
    "FIntPhysicsGridHierarchyLowestLevelInitBinCountWorldModel": "100000000",
    "FIntPhysicsSolverCollisionPoolBucketSize": "2147483647",
    "FIntPhysicsSolverCollisionPoolBucketSizeWorldModel": "2147483647"
}
```
### Crash Roblox 1
```json
{
    "DFIntTimestepArbiterThresholdCFLThou": "0"
}
```
### Crash Roblox 2
```json
{
    "DFFlagVideoCaptureServiceEnabled": "False"
}
```
### Increase Ping 
```json
{
    "DFIntDataSenderMaxBandwidthBps": "150"
}
```
### Crash roblox 3 
##### when you try to launch roblox it won't open
```json
{
    "DFFlagDebugSimulateHangAtStartup": "True"
}
```
### Crash roblox 4
##### the same thing from above but it only crashes when you try to close roblox
```json
{
    "DFFlagDebugSimulateHangAtShutdown": "True"
}
```
<h1 align="center">Debug</h1>

### Shows the state of a flag
```json
{
    "FStringDebugShowFlagState": "FLAG_HERE"
}
```
###### e.g
```json
{
    "FStringDebugShowFlagState": "DFIntTaskSchedulerTargetFps, ChannelName"
}
```
### Show Outlined Chunks
```json
{
    "FFlagDebugLightGridShowChunks": "True"
}
```
### Show Outlined Chunks that are being interacted
```json
{
    "DFFlagDebugEnableStreamingSolverVisualization": "True"
}
```
### Prevents Remote Events from running
```json
{
    "DFIntRemoteEventSingleInvocationSizeLimit": "1"
}
```
### log player joins,leaves,messages
###### only works with the new chat
###### @return_request
```json
{
    "FStringDebugLuaLogLevel": "trace",
    "FStringDebugLuaLogPattern": "ExpChat/mountClientApp"
}
```
### Octree Validation
```json
{
    "FFlagDebugEnableOctreeValidation": "True"
}
```
### Self Explanatory 1
```json
{
    "DFFlagDebugPrintDataPingBreakDown": "True"
}
```
### Self Explanatory 2
```json
{
    "DFFlagDebugAudioLogging": "True"
}
```
### Duplicate of Above
```json
{
    "DFFlagDebugAudioLogging2": "True"
}
```
### Self Explanatory 3
```json
{
    "FFlagTrackerLodControllerDebugUI": "True"
}
```
### Self Explanatory 4
###### Disable Drag Detectors
```json
{
    "FFlagDragDetectors1": "False"
}
```
### Self Explanatory 5
###### Disabe CTM Climbing
```json
{
    "FFlagUserClickToMoveSupportAgentCanClimb2": "False"
}
```
### Self Explanatory 6
###### Disabe Feedback Button in ESC
```json
{
    "FFlagDisableFeedbackSoothsayerCheck": "False"
}
```
### Self Explanatory 7
###### LDL dev console printing
###### @tyetonix
```json
{
    "DFFlagDebugSimLDLProgramPrintBuildStats": "True",
    "DFFlagDebugSimLDLProgramPrintExecStats": "True"
}
```
### Self Explanatory 8
###### prints body allocations counts in dev console
###### @tyetonix
```json
{
    "FFlagDebugCountSimBodyAllocations": "True"
}
```
### Max dev console log count
###### Control how many developer console logs can be shown at once, for example if you set the limit to be 100, then 100 different log messages will be shown while any older ones will be deleted when the limit is reached
###### @satlybpro
```
{
    "FIntNewDevConsoleMaxLogCount": "2147483647"
}
```
### Self Explanatory 13
###### Default value is 650, higher value more usage lower value less
```json
{
    "FIntRenderMaxShadowAtlasUsageBeforeDownscale": "650"
}
```
### Self Explanatory 14
###### Allows you to edit the DataModel Patch
```
{
    "FFlagDataModelPatcherForceLocal": "True"
}
```
### Limit console message length
###### changes the max character length limit for each dev console message
###### @satlybpro
```
{
    "FIntStandardOutputMaximumCharacterLength": "100"
}
```
### Replace all Decals with a Test Image
###### @.rbx.bloxy
```json
{
    "FFlagDebugTestImageDrawItem": "True"
}
```

<h1 align="center">Community Presets</h1>

<h4 align="center">We are not accepting performance Fast Flags that aren't listed or known.</h4>

### absolutely kill your game quality with fflags known to me
##### @dynamitebumblemouth
```json
{
    "FFlagDisablePostFx": "True",
    "FIntDebugTextureManagerSkipMips": "8",
    "DFIntTextureCompositorActiveJobs": "0",
    "DFIntCSGLevelOfDetailSwitchingDistance": "0",
    "DFIntCSGLevelOfDetailSwitchingDistanceL12": "0",
    "DFIntCSGLevelOfDetailSwitchingDistanceL23": "0",
    "DFIntCSGLevelOfDetailSwitchingDistanceL34": "0",
    "DFIntDebugFRMQualityLevelOverride": "1",
    "DFFlagDebugPauseVoxelizer": "True",
    "DFFlagDebugRenderForceTechnologyVoxel": "True",
    "FFlagGlobalWindRendering": "False",
    "FIntRenderShadowIntensity": "0",
    "FIntRenderShadowmapBias": "1",
    "FIntDebugForceMSAASamples": "-1",
    "FIntFRMMinGrassDistance": "0",
    "DFIntTextureQualityOverride": "1"
}
```
