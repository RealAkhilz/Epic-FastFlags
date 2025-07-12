> [!important]
> https://discord.gg/rGdPF82Tmf

<h1 align="center">
  <img src="https://raw.githubusercontent.com/bloxstraplabs/bloxstrap/main/Images/Bloxstrap.png" width="30"> Epic FastFlags
</h1>

<h3 align="center"> Made by <a href="https://guns.lol/realakhil">RealAkhilz</a> </h3>

<h5>Version 1.0.5 [7/12/2025]</h5>

  - Added quick navigation
  - Added custom emojis

- - -

<h2> 
  <img src="https://github.com/RealAkhilz/Epic-FastFlags/blob/main/assets/emojis/IconRocket.png" width="30"> Quick Links 
</h2>

<div align="center">

[![guns.lol](https://img.shields.io/badge/guns.lol-RealAkhilz-darkblue?style=flat&logo=link&logoColor=white)](https://guns.lol/realakhil)
[![GitHub stars](https://img.shields.io/github/stars/RealAkhilz/Epic-FastFlags?style=social)](https://github.com/RealAkhilz/Epic-FastFlags)
[![Discord](https://img.shields.io/discord/1380077621974667264?label=Discord&color=5865F2&logo=discord&logoColor=white)](https://discord.gg/848BdgmvD9)

</div>

- - -

<h2>
  <img src="https://github.com/RealAkhilz/Epic-FastFlags/blob/main/assets/emojis/IconPlus.png" width="30"> How to import fastflags
</h2>

- **Open ur bootstrapper**
- **Fast Flags >> Add new >> Import JSON**
- **Paste in JSON**
- **Save the settings and u should be good to go!**

<img src="https://raw.githubusercontent.com/RealAkhilz/Epic-FastFlags/main/assets/tutorial.gif" >

- - -

<h2>
  <img src="https://github.com/RealAkhilz/Epic-FastFlags/blob/main/assets/emojis/IconStars.png" width="30"> FastFlags
</h2>

> [!Warning]  
> Some fastflags have !Important, !Warning, and !Caution, please read the fastflags that have these and use fastflags wisely.

> [!Important]
> FastFlags do NOT get u banned of Roblox. U will only get banned if u use abusive/cheating FastFlags

<h3>
  <img src="https://github.com/RealAkhilz/Epic-FastFlags/blob/main/assets/emojis/IconStars.png" width="25"> Quick Navigation
</h3>

- [Rendering API](https://github.com/RealAkhilz/Epic-FastFlags?tab=readme-ov-file#rendering-api)
- [Graphics and Rendering FastFlags](https://github.com/RealAkhilz/Epic-FastFlags?tab=readme-ov-file#graphic-and-rendering-fastflags)
- [Lighting](https://github.com/RealAkhilz/Epic-FastFlags?tab=readme-ov-file#lighting)
- [Graphical Settings](https://github.com/RealAkhilz/Epic-FastFlags?tab=readme-ov-file#graphical-settings)
- [UI](https://github.com/RealAkhilz/Epic-FastFlags?tab=readme-ov-file#ui)
- [Audio](https://github.com/RealAkhilz/Epic-FastFlags?tab=readme-ov-file#audio)
- [Latency](https://github.com/RealAkhilz/Epic-FastFlags?tab=readme-ov-file#latency)

## Rendering API

### Direct3D 11

```json
{
  "FFlagRenderEnableGlobalInstancingD3D11": "true",
  "FFlagDebugGraphicsPreferD3D11": "true",
  "FFlagGraphicsD3D11ExtraInitLog": "false",
  "FFlagDebugGraphicsDisableDirect3D11": "false",
  "FIntRenderShaderLoadAnalyticsHundredthPercent": 0,
  "FFlagDisableHQShadersLowEndDx11": "true",
  "FIntRenderDx11LowEndCoreCount": "SET THE VALUE TO YOUR CPU CORES"
}
```

### Direct3D 10

```json
{
  "FFlagDebugGraphicsPreferD3D11FL10": "true",
  "FFlagGraphicsEnableD3D10Compute": "true",
  "FFlagRenderEnableGlobalInstancingD3D10": "true",
  "FFlagRenderEnableGlobalInstancingD3D11": "false"
}
```

### Metal

> [!NOTE]  
> This rendering API is only for macOS.

```json
{ "FFlagDebugGraphicsPreferMetal": "True" }
```

### Vulkan (Linux and Android)

```json
{
  "FIntGraphicsVulkanAnalyticsHundredthPercent": "0",
  "FFlagVulkanAlwaysLogLayersAndExtensions": "false",
  "FIntGraphicsVulkanARMVaryingBufferMb": "1024",
  "FIntGraphicsVulkanBonusMemoryCPU": "100",
  "FIntGraphicsVulkanBonusMemoryGPU": "100",
  "FFlagDebugGraphicsDisableDirect3D11": "True",
  "FFlagDebugGraphicsDisableVulkan": "False",
  "FFlagDebugGraphicsPreferVulkan": "True",
  "FFlagGraphicsVulkanBonusMemory": "True",
  "FFlagRenderEnableGlobalInstancingVulkan": "True",
  "FFlagDebugVulkanDisablePreRotate": "False",
  "FStringGraphicsVulkanAdrenoFutureDeviceBlacklist": null,
  "FStringGraphicsVulkanAdrenoFutureDriverBlacklist": null,
  "FStringGraphicsVulkanFutureGPUNameBlacklist": null,
  "FStringGraphicsVulkanMaliFutureDeviceBlacklist": null,
  "FStringGraphicsVulkanMaliFutureDriverBlacklist": null,
  "FStringGraphicsVulkanPVRFutureDeviceBlacklist": null,
  "FStringGraphicsVulkanPVRFutureDriverBlacklist": null,
  "FStringGraphicsVulkanVaryingBufferLimitMiB": "0x13B5:.+:.+=1024;0x5143:.+:.+=1024",
  "FStringVulkanBuggyRenderpassList2": "YOUR GPU NAME"
}
```

### OpenGL

```json
{
  "FFlagDebugGraphicsDisableDirect3D11": "true",
  "FFlagDebugGraphicsPreferOpenGL": "true",
  "FFlagGraphicsGLEnableHQShadersExclusion": "true",
  "FFlagGraphicsGLEnableSuperHQShadersExclusion": "true"
}
```

## Graphic and Rendering FastFlags

### Kilo Pixels

> [!NOTE]  
> This fastflag changes Roblox resolution in kilo pixels, like the YouTube graphics slider (Roblox GUI and game UI unaffected).

```
4320p (8k) - 33178
2160p (4k) - 8294
1440p (2K) - 3686
1080p (FHD) - 2074
720p (HD) - 922
480p (SD) - 410
360p (Low SD) - 230
```

```json
{ "DFIntDebugDynamicRenderKiloPixels": "-1" }
```

### Disable Post-Processing

> [!NOTE]  
> This fastflag disables post-processing.

```json
{ "FFlagDisablePostFx": "True" }
```

### Minimal Rendering

> [!NOTE]  
> Renders certain terrain and textures at a lower quality, potentially improving performance.

```json
{ "FFlagDebugRenderingSetDeterministic": "True" }
```

### Preserve Rendering Quality With Display Setting

> [!NOTE]  
> Roblox reduces your rendering quality depending on how your display is scaled in Windows.

```json
{ "DFFlagDisableDPIScale": "True" }
```

### Disable Textures

> [!NOTE]  
> This fastflag disables Roblox textures.

```json
{ "FFlagTextureUseACR3": "True", "FIntTextureUseACRHundredthPercent": "10000" }
```

### Low Poly Meshes

> [!NOTE]  
> Makes poly meshes low quality.

```json
{
  "DFIntCSGLevelOfDetailSwitchingDistance": "0",
  "DFIntCSGLevelOfDetailSwitchingDistanceL12": "0",
  "DFIntCSGLevelOfDetailSwitchingDistanceL23": "0",
  "DFIntCSGLevelOfDetailSwitchingDistanceL34": "0"
}
```

### Disable Player Shadows

> [!NOTE]  
> This fastflag disables player shadows.

```json
{ "FIntRenderShadowIntensity": "0" }
```

## Lighting

### Voxel Lighting (Phase 1)

```json
{ "DFFlagDebugRenderForceTechnologyVoxel": "true" }
```

### Feature VoxelGrid ❗

> [!CAUTION]  
> Visual Crashes & Buggy

```json
{ "FFlagVoxelGridNew6": "true" }
```

### Shadowmap Lighting (Phase 2)

```json
{ "FFlagDebugForceFutureIsBrightPhase2": "true" }
```

### Future Lighting (Phase 3)

```json
{ "FFlagDebugForceFutureIsBrightPhase3": "true" }
```

### Unified Lighting (LightGrid - Beta)

```json
{ "FFlagRenderUnifiedLighting15": "true" }
```

### Unified Lighting Blend Zone

```json
{ "FIntUnifiedLightingBlendZone": "400" }
```

## Graphical Settings

### Reset Cache On Game Leave

> [!NOTE]  
> In game engines, a cache is a temporary storage location for frequently accessed data, designed to speed up game performance by reducing the time it takes to retrieve information. Clearing the cache can improve game performance, fix loading errors, and resolve connectivity problems.

```json
{ "FFlagResetCacheOnLeaveGame": "true" }
```

### Optimize CFrame Update

> [!NOTE]  
> Reduces CPU and GPU usage.

```json
{
  "FFlagOptimizeCFrameUpdates4": "true",
  "FFlagOptimizeCFrameUpdatesIC4": "true"
}
```

### Stop Being Jumpscared

```json
{ "DFFlagJumpScaresP2": "false" }
```

### Improved Object Detail

> [!NOTE]  
> FractalUpsample - Fractal upsampling is a technique used to increase the resolution or detail of an image, texture, or grid by applying fractal algorithms. Unlike traditional upscaling methods that simply stretch the original content, fractal upsampling generates new details based on mathematical fractal patterns. These patterns mimic natural complexity, allowing the upsampled image or grid to retain a more realistic or detailed appearance.

```json
{
  "FFlagDebugGridForceFractalUpsample": "true",
  "DFFlagRenderLanczosUpsamplingNonRinging2": "true",
  "DFFlagRenderSmootherStepUpsampling2": "true"
}
```

### Custom Record Video Roblox

> [!NOTE]  
> Default = 30 FPS and 2M bit on 1 video 🤣🤣🤣

```json
{
  "DFIntCaptureVideoMaxFrameRate": 60,
  "DFIntCaptureVideoBitrate": 8000000
}
```

### Quaternion Corrections Animations

> [!NOTE]  
> Applies quaternion-based corrections to character/object poses, helping ensure smoother and more accurate rotations, particularly during complex animations or movements.

```json
{
  "FFlagKeyframeSequenceUseRuntimeSyncPrims": "true",
  "FFlagQuaternionPoseCorrection": "true"
}
```

### Multithreading Improvement

> [!NOTE]  
> Basically makes Roblox use as many threads as you put there (+1 because of main/render thread). However, this is poorly made (L Roblox); it actually just switches between the threads really quickly, causing overhead.  
> What I recommend is setting this to 1 so it uses 2 worker threads + the main thread (won’t go lower than this). If you have a decent CPU, this can improve your FPS (it did for me).  
> Default = 3

```json
{ "DFIntRuntimeConcurrency": "your core+1" }
```

### Fast Preloading Everything

> [!NOTE]  
> This improves loading time speeds for games.

```json
{
  "DFFlagEnableMeshPreloading2": "true",
  "DFFlagEnableMeshPreloading": "true",
  "DFFlagEnableTexturePreloading": "true",
  "DFFlagEnableSoundPreloading": "true",
  "FFlagAssetPreloadingIXP": "true",
  "DFIntAssetPreloading": "9999999",
  "DFIntNumAssetsMaxToPreload": "9999999"
}
```

### Removes Only Roblox Texture

```json
{
  "FFlagTextureUseACR5": "true",
  "FFlagTexturePackUseACR4": "true",
  "FIntTextureUseACRHundredthPercent": "10000"
}
```

### No Unaligned DXT

> [!NOTE]  
> DXT (also known as S3TC) is a texture compression format. It’s widely supported on most GPUs and helps textures stay compressed while in video memory. This allows users to use more or larger textures. Unaligned DXT can cause performance issues on some low-end or unsupported GPUs.

```json
{ "FStringGraphicsDisableUnalignedDxtGPUNameBlacklist": "YOUR_GPU" }
```

### Configure FRM Refresh Rate

> [!NOTE]  
> 120Hz

```json
{
  "DFIntGraphicsOptimizationModeFRMFrameRateTarget": "120",
  "DFIntGraphicsOptimizationModeMinFrameTimeTargetMs": "10",
  "DFIntGraphicsOptimizationModeMaxFrameTimeTargetMs": "17"
}
```

> [!NOTE]  
> 144Hz

```json
{
  "DFIntGraphicsOptimizationModeFRMFrameRateTarget": "144",
  "DFIntGraphicsOptimizationModeMinFrameTimeTargetMs": "8",
  "DFIntGraphicsOptimizationModeMaxFrameTimeTargetMs": "10"
}
```

> [!NOTE]  
> 165Hz

```json
{
  "DFIntGraphicsOptimizationModeFRMFrameRateTarget": "165",
  "DFIntGraphicsOptimizationModeMinFrameTimeTargetMs": "7",
  "DFIntGraphicsOptimizationModeMaxFrameTimeTargetMs": "9"
}
```

> [!NOTE]  
> 180Hz

```json
{
  "DFIntGraphicsOptimizationModeFRMFrameRateTarget": "180",
  "DFIntGraphicsOptimizationModeMinFrameTimeTargetMs": "6",
  "DFIntGraphicsOptimizationModeMaxFrameTimeTargetMs": "8"
}
```

> [!NOTE]  
> 240Hz

```json
{
  "DFIntGraphicsOptimizationModeFRMFrameRateTarget": "240",
  "DFIntGraphicsOptimizationModeMinFrameTimeTargetMs": "5",
  "DFIntGraphicsOptimizationModeMaxFrameTimeTargetMs": "6"
}
```

### Disable Render Shadow Huge Radius

```json
{ "DFIntRenderShadowHugeRadius": "0" }
```

### Fast Render ❗

> [!WARNING]  
> More Laggy

```json
{ "FIntRenderFastCluster": "255" }
```

### Render Mesh Optimize

```json
{ "FIntRenderMeshOptimizeVertexBuffer": "1" }
```

### Pixel Quality Roblox

> [!NOTE]  
> 144p = 37  
> 240p = 77  
> 360p = 230  
> 480p = 410  
> 720p = 922  
> 1080p = 2074  
> 1440p = 3686  
> 2160p (4k) = 8294  
> 4320p (8k) = 33178

```json
{ "DFIntDebugDynamicRenderKiloPixels": "410" }
```

### Remove Rendering Pre Processor

```json
{ "FFlagRemovedRbxRenderingPreProcessor": "true" }
```

### Max Shadow Atlas Usage Before Downscale

> [!NOTE]  
> You can change number and work with Unified Lighting.

```json
{ "FIntRenderMaxShadowAtlasUsageBeforeDownscale": "-1" }
```

### Disable Highlights on Parts

```json
{ "DFFlagRenderHighlightManagerPrepare4": "true" }
```

### Legacy Shadow

```json
{ "FFlagRenderLegacyShadowsQualityRefactor": "true" }
```

### SSAO (Screen-Space Ambient Occlusion)

```json
{ "FFlagDebugSSAOForce": "true" }
```

### Smoother Terrain ❗

> [!CAUTION]  
> The particle's speed is based on your FPS.

```json
{
  "FFlagRenderFixParticleDegenCrossProduct": "true",
  "FFlagDebugRenderingSetDeterministic": "true"
}
```

### Speed up Particle Emitters ❗

> [!CAUTION]  
> The particle's speed is based on your FPS.

```json
{
  "FFlagRenderFixParticleDegenCrossProduct": "true",
  "FFlagDebugDeterministicParticles": "true"
}
```

### Custom Threads

> [!NOTE]  
> You can use it or Roblox default.

```json
{
  "FIntTaskSchedulerThreadMin": "0",
  "FIntRuntimeMaxNumOfThreads": "1800"
}
```

### Fully Enable HyperThreading

```json
{
  "FFlagDebugCheckRenderThreading": "true",
  "FFlagRenderDebugCheckThreading2": "true"
}
```

### Fully Enable MovePrerender ❗

> [!WARNING]  
> Lag, stuttering = remove it.

```json
{
  "FFlagMovePrerender": "true",
  "FFlagMovePrerenderV2": "true"
}
```

### Force Graphics Quality Level

> [!NOTE]  
> Note: 1-21

```json
{ "FIntRomarkStartWithGraphicQualityLevel": "1" }
```

### Low Graphics Quality w/ Max Render Distance/FRM Quality Levels

> [!NOTE]  
> Explanation: 1-6 Are low graphics, Above 6 are high graphics. Like the 1-21 graphics slider.

```json
{ "DFIntDebugFRMQualityLevelOverride": "1" }
```

### Low Render Distance

> [!NOTE]  
> Only works if game has StreamingEnabled.

```json
{ "DFIntDebugRestrictGCDistance": "1" }
```

### FRM Levels

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

### Disables Fade In and Fade Out Animation Every Light Update

```json
{ "FIntRenderLocalLightFadeInMs": "0" }
```

### Custom Limits Light Updates

> [!NOTE]  
> You can use it or Roblox Default.

```json
{
  "FIntRenderLocalLightUpdatesMin": "0",
  "FIntRenderLocalLightUpdatesMax": "8"
}
```

### Force LOD on Meshes

> [!NOTE]  
> Not recommended for Evade players. Weird map.

```json
{
  "DFIntCSGLevelOfDetailSwitchingDistance": "0",
  "DFIntCSGLevelOfDetailSwitchingDistanceL12": "0",
  "DFIntCSGLevelOfDetailSwitchingDistanceL23": "0",
  "DFIntCSGLevelOfDetailSwitchingDistanceL34": "0"
}
```

### White Everything

```json
{ "FFlagSkyUseRGBEEncoding": "true" }
```

### Black Wall ❗

> [!CAUTION]  
> Very Buggy

```json
{ "FIntCameraFarZPlane": "60" }
```

### Disable Feature Sky

```json
{
  "FFlagAdvSkyUsesRuntime": "false",
  "FFlagSkyboxOrientation": "false",
  "DFFlagFixSkyBoxTextureBlurriness": "false"
}
```

### Gray Sky

> [!NOTE]  
> You can use it or Roblox Default.

```json
{ "FFlagDebugSkyGray": "true" }
```

### White Sky ❗

> [!WARNING]  
> Only applies to games with the default skybox.

```json
{
  "FFlagDebugSkyGray": "true",
  "FFlagSkyUseRGBEEncoding": "true"
}
```

### Colorful Sky ❗

> [!CAUTION]  
> Very Buggy

```json
{
  "DFFlagTextureQualityOverrideEnabled": "true",
  "DFIntTextureQualityOverride": "0",
  "FIntDebugFRMOptionalMSAALevelOverride": "0",
  "FIntVertexSmoothingGroupTolerance": "0",
  "FIntDebugTextureManagerSkipMips": "8",
  "FIntDebugForceMSAASamples": "0"
}
```

### Black Sky

```json
{
  "FIntDebugTextureManagerSkipMips": "8",
  "DFIntTextureQualityOverride": "0",
  "FIntVertexSmoothingGroupTolerance": "10000",
  "DFFlagTextureQualityOverrideEnabled": "true"
}
```

### Pause Voxelizer/Disable Baked Shadows ❗

> [!WARNING]  
> If you play horror games, I don’t recommend you use it.

```json
{ "DFFlagDebugPauseVoxelizer": "true" }
```

### Skip Mesh Voxelizer

```json
{ "DFFlagDebugSkipMeshVoxelizer": "true" }
```

### Enable CPULightCulling

```json
{ "FFlagDebugForceFSMCPULightCulling": "true" }
```

### Enable GPULightCulling

> [!NOTE]  
> Combine with [Lighting Attenuation] for better vision.

```json
{ "FFlagFastGPULightCulling3": "true" }
```

### Lighting Attenuation ❗

> [!CAUTION]  
> Weird Lighting

```json
{ "FFlagNewLightAttenuation": "true" }
```

### Custom Frame Buffer

```json
{
  "DFIntMaxFrameBufferSize": "4",
  "FIntInterpolationAwareTargetTimeLerpHundredth": "100",
  "FIntMaquettesFrameRateBufferPercentage": "100",
  "DFIntMaxAverageFrameDelayExceedFactor": "0"
}
```

### Low Quality Terrain Textures

> [!NOTE]  
> 0 -> 4 for less quality, 16, 32, 64 for higher quality.

```json
{ "FIntTerrainArraySliceSize": "0" }
```

### High Quality Textures

> [!NOTE]  
> 1 -> 3

```json
{
  "DFFlagTextureQualityOverrideEnabled": "True",
  "DFIntTextureQualityOverride": "3"
}
```

### Lower Quality Textures

```json
{ "DFIntPerformanceControlTextureQualityBestUtility": "-1" }
```

### No Avatar Textures

```json
{ "DFIntTextureCompositorActiveJobs": "0" }
```

### Texture Manager

> [!NOTE]  
> 1-4 Blurry, 5-7 low quality also removes studs, 8-10 Removes almost everything (this is better).

```json
{ "FIntDebugTextureManagerSkipMips": "10" }
```

### Remove Grass

```json
{
  "FIntFRMMinGrassDistance": "0",
  "FIntFRMMaxGrassDistance": "0",
  "FIntRenderGrassDetailStrands": "0"
}
```

### No Grass Motion

```json
{ "FIntGrassMovementReducedMotionFactor": "0" }
```

### Increased Grass Motion

```json
{ "FIntGrassMovementReducedMotionFactor": "999" }
```

### Force MSAA

> [!NOTE]  
> 1 -> 7

```json
{
  "FIntDebugForceMSAASamples": "1",
  "FIntDebugFRMOptionalMSAALevelOverride": "1"
}
```

### ShadowMap Bias

> [!NOTE]  
> [Future & ShadowMap]

```json
{ "FIntRenderShadowmapBias": "-1" }
```

### Disable Dynamic Heads Animations

> [!NOTE]  
> https://roblox.fandom.com/wiki/Dynamic_Head

```json
{
  "DFIntAnimationLodFacsDistanceMin": "0",
  "DFIntAnimationLodFacsDistanceMax": "0",
  "DFIntAnimationLodFacsVisibilityDenominator": "0"
}
```

### Remove Head Roll Limit for Face Tracking

> [!NOTE]  
> Server Sided Only

```json
{ "DFIntAvatarFaceChatHeadRollLimitDegrees": "360" }
```

### Remove Layered Clothing Related for Searching in Lua App Catalog

```json
{ "FStringAXCategories": "ClassicShirts.ClassicTShirts.ClassicPants" }
```

### Quick Game Launch ❗

> [!CAUTION]  
> BUG: Can’t load full item avatar.

```json
{ "FFlagEnableQuickGameLaunch": "true" }
```

### Enable Highlight Outlines on Any Rendering API ❗

> [!WARNING]  
> Lags a bit, use if you love highlights.

```json
{
  "FFlagHighlightOutlinesOnMobile": "true",
  "DFFlagVisBugHighlightImprovement": "true"
}
```

### Enable GPU Texture Compressor

```json
{ "FFlagRenderGpuTextureCompressor": "true" }
```

### Enable HSR (Hidden Surface Removal)

> [!NOTE]  
> It works like occlusion culling.

```json
{
  "FFlagDebugForceGenerateHSR": "true",
  "FFlagDebugApplyHSRForTransparentMesh": "true",
  "FFlagHSRClusterImprovement": "true",
  "FFlagHSRRemoveDuplicateIndices": "true"
}
```

### Simulation Optimization Flag

```json
{
  "FFlagSimDcdEnableLAR2": "true",
  "FFlagSimDcdRefactorDelta3": "true",
  "DFIntBufferCompressionLevel": "0",
  "DFIntBufferCompressionThreshold": "100",
  "DFIntPerformanceControlFrameTimeMax": "1",
  "DFIntPerformanceControlFrameTimeMaxUtility": "-1",
  "FFlagPushFrameTimeToHarmony": "true",
  "DFIntAnimatorThrottleMaxFramesToSkip": "0",
  "DFIntNumFramesAllowedToBeAboveError": "0",
  "DFIntVisibilityCheckRayCastLimitPerFrame": "10",
  "DFIntNetworkSchemaCompressionRatio": "50",
  "DFIntTimeBetweenSendConnectionAttemptsMS": "50"
}
```

### Network CPU RSS Tweaks

```json
{
  "DFIntPhysicsReceiveNumParallelTasks": "20",
  "DFIntPhysicsAnalyticsHighFrequencyIntervalSec": "20",
  "FIntSimWorldTaskQueueParallelTasks": "20",
  "FIntSmoothClusterTaskQueueMaxParallelTasks": "20",
  "DFIntReplicationDataCacheNumParallelTasks": "20",
  "DFIntMegaReplicatorNumParallelTasks": "20"
}
```

### Vertex Smoothing Group Tolerance ❗

> [!WARNING]  
> The FIntVertexSmoothingGroupTolerance flag controls the tolerance level for vertex smoothing groups in 3D graphics. Lower values result in lower smoothing quality as more errors are tolerated, making models appear more angular and less smooth. Higher values increase the smoothing accuracy, leading to smoother, more visually appealing models with fewer artifacts.

```json
{ "FIntVertexSmoothingGroupTolerance": "1000" }
```

### Better Shadows ❗

> [!WARNING]  
> Loading will take longer, but the shadows are much better.

```json
{ "FFlagRenderInitShadowmaps": "true" }
```

### Raycast Performance Improvements

> [!NOTE]  
> https://create.roblox.com/docs/workspace/raycasting

```json
{ "FFlagUserRaycastPerformanceImprovements": "true" }
```

### Shoe Skip Render Mesh

```json
{ "FFlagShoeSkipRenderMesh": "true" }
```

### New Version of Render

> [!NOTE]  
> Enables an updated rendering system to improve performance and manage render calls.

```json
{ "FFlagRenderCBRefactor2": "true" }
```

### Directional Attenuation Max Points ❗

> [!WARNING]  
> Lower values: May improve performance but reduce lighting accuracy. Higher values: Increase lighting accuracy at the cost of performance, potentially leading to slower rendering, especially in scenes with complex lighting setups.  
> Explanation: Limits the maximum number of sample points for calculating directional light attenuation. Lower values improve performance but may reduce lighting accuracy. Higher values increase lighting accuracy but may slow rendering in complex lighting setups.

```json
{ "FIntDirectionalAttenuationMaxPoints": "400" }
```

### Simulation Optimization Flag

> [!NOTE]  
> Be mindful that while optimization can improve performance, it may also require testing to ensure that the behavior of sets remains consistent and that no necessary details are lost during the optimization process. The DFFlagSimOptimizeSetSize flag is used to optimize the size of sets in simulations. Enabling this flag activates optimization techniques that reduce the size of simulation sets, leading to better performance by decreasing memory usage and potentially improving processing speeds during simulations.

```json
{ "DFFlagSimOptimizeSetSize": "true" }
```

### Makes Avatars Shiny

```json
{
  "DFIntRenderClampRoughnessMax": "-640000000",
  "DFIntDebugFRMQualityLevelOverride": "6"
}
```

### Limits Number of Animations Being Played ❗

```json
{ "DFIntMaxActiveAnimationTracks": "0" }
```

### Remove Bloom

```json
{
  "FIntBloomFrmCutoff": "1654515",
  "FFlagRenderNoLowFrmBloom": "true"
}
```

### Telemetry

#### Remove Minimum Required Memory For Roblox

```json
{
  "FIntMininumRequiredMemoryInGB": "0",
  "FIntMininumRequiredMemoryInMB": "0"
}
```

#### Zero Telemetry

```json
{
  "DFStringTelemetryV2Url": "0.0.0.0",
  "DFStringHttpPointsReporterUrl": "null",
  "FFlagEnableServiceInitBreakdownTelemetry": "false",
  "DFFlagReportReplicatorStatsToTelemetryV22": "false",
  "DFFlagDebugDisableTelemetryAfterTest": "true",
  "FFlagEnableTelemetryProtocol": "false",
  "FFlagEnableTelemetryService1": "false",
  "FFlagOpenTelemetryEnabled2": "false",
  "FLogRobloxTelemetry": "0",
  "FFlagTimeAndNewJoinDataTelemetry": "false",
  "FFlagDisableMemoryTracking": "true",
  "DFStringRobloxAnalyticsURL": "null",
  "FFlagLuaAppDesktopMediaGalleryTelemetry": "false",
  "FFlagMediaAccordionAndFullTelemetry": "false",
  "DFStringRobloxTelemetryReliabilityCountAllowList": "null"
}
```

#### Disable Telemetry by China and VNG

```json
{
  "FFlagEnableVNGNewAppAvailableModal": "false",
  "FFlagLuaAppHomeVngAppUpsell": "false",
  "FFlagVngTOSRevisedEnabled": "false",
  "FStringVNGWebshopUrl": "null",
  "FStringTencentAuthPath": "null",
  "FLogTencentAuthPath": "false",
  "FStringDevPublishChinaRequirementsLink": "null",
  "FLogDevPublishChinaRequirementsLink": "false"
}
```

#### Don’t Give Roblox Info On Your Device

```json
{
  "DFIntReportDeviceInfoRate": 0,
  "DFIntReportOutputDeviceInfoEventRateHundredthsPercentage": 0,
  "DFIntReportOutputDeviceInfoRateHundredthsPercentage": 0,
  "DFIntReportRecordingDeviceInfoEventRateHundredthsPercentage": 0,
  "DFIntReportRecordingDeviceInfoRateHundredthsPercentage": 0
}
```

### Disable In-Game Advertisements

```json
{
  "FFlagAdServiceEnabled": "false",
  "FLogAdService": 0
}
```

### Disable Events Tab/Change Its URL

```json
{
  "FFlagPlatformEventEnabled2": "false",
  "FStringPlatformEventUrl": "https://www.google.com/"
}
```

### Disable In-Game Purchases

```json
{ "DFFlagOrder66": "true" }
```

### Disable Chat

```json
{ "FFlagDebugForceChatDisabled": "true" }
```

### Disable Voice Chat

> [!NOTE]  
> Setting this to True will not do anything.  
> [TIP] Use PlaceFilter for specific games.

```json
{ "DFFlagVoiceChat4": "false" }
```

### Log Chat Yourself

```json
{ "FFlagDebugShowTextBounds": "true" }
```

### Overlay That Shows What You Type

```json
{ "FFlagDebugTextBoxServiceShowOverlay": "true" }
```

### Disable Bubble Chat

```json
{ "FFlagEnableBubbleChatFromChatService": "false" }
```

## Quality of Life

### Unlimited FPS Unlocker

```json
{
  "FFlagTaskSchedulerLimitTargetFpsTo2402": "false",
  "FFlagGameBasicSettingsFramerateCap5": "false",
  "DFIntTaskSchedulerTargetFps": "9999"
}
```

### GUI Hiding Toggles

```json
{
  "FFlagUserShowGuiHideToggles": "true",
  "FFlagGuiHidingApiSupport2": "true"
}
```

#### Key Combinations

```
Ctrl + Shift + B: Toggles GUIs in 3D space (BillboardGuis, SurfaceGuis, etc)
Ctrl + Shift + C: Toggles game-defined ScreenGuis
Ctrl + Shift + G: Toggles Roblox CoreGuis
Ctrl + Shift + N: Toggles player names, and other BillboardGuis that show up above a player
```

```json
{ "DFIntCanHideGuiGroupId": "ID" }
```

### Disable Fullscreen Title Bar

```json
{ "FIntFullscreenTitleBarTriggerDelayMillis": "3600000" }
```

### Spammed Letters ❗

> [!WARNING]  
> This flag basically spams every other letter on Roblox CoreGUI and the game's GUI but it doesn't affect some parts of the games!  
> Default is 0, and if you set it to anything higher, it just follows whatever number you put.

```json
{ "FIntDebugTextElongationFactor": "999999" }
```

### MTU ❗

> [!WARNING]  
> 700 -> 1500  
> Risks caused by yourself.

```json
{ "DFIntConnectionMTUSize": "MTU_HERE" }
```

### No Internet Disconnect ❗

> [!CAUTION]  
> You will still be kicked, but the message won’t show.

```json
{ "DFFlagDebugDisableTimeoutDisconnect": "true" }
```

### Smoother/Faster Input

> [!NOTE]  
> Tip: When enabled, the game will use an updated implementation for processing user input, which may lead to smoother and more responsive interactions. This flag controls the refactoring of the legacy input handling system in Roblox.  
> Recommendation: Test your game thoroughly after enabling this flag to ensure that everything functions as expected.

```json
{ "FFlagLuaAppLegacyInputSettingRefactor": "true" }
```

### Disable New Chat Report

```json
{ "DFFlagChatLineAbuseReportAPIEnabled2": "false" }
```

### Stuttery Animation Fix

```json
{ "DFIntTimestepArbiterThresholdCFLThou": "300" }
```

### Surf the Web Inside of Roblox

> [!NOTE]  
> Click the Beta badge or the 13+ badge to open the webview browser.

```json
{
  "FFlagTopBarUseNewBadge": "true",
  "FStringTopBarBadgeLearnMoreLink": "https://google.com/",
  "FStringVoiceBetaBadgeLearnMoreLink": "https://google.com/"
}
```

### Adjust Default Timeout Time

> [!NOTE]  
> 1 second = 1000

```json
{ "DFIntDefaultTimeoutTimeMs": "5000" }
```

### Automatically Unmutes Your Mic on Join (VC)

```json
{ "FFlagDebugDefaultChannelStartMuted": "false" }
```

### Lets You Change the Zoom Out Limit

> [!NOTE]  
> Only applies to games that have not changed the default zoom limit.

```json
{ "FIntCameraMaxZoomDistance": "9999" }
```

### Exclusive Fullscreen

```json
{ "FFlagHandleAltEnterFullscreenManually": "false" }
```

### Remove Translated Supported Message on Join

```json
{ "FFlagChatTranslationEnableSystemMessage": "false" }
```

### Always Display Render Stats

> [!NOTE]  
> Pretty self-explanatory flag; you can't disable them using the hotkey.

```json
{ "FFlagDebugAlwaysDisplayRenderStats": "true" }
```

### Subscriptions Page

```json
{
  "FFlagLuaAppDevSubsEnabled": "true",
  "DFFlagDeveloperSubscriptionsEnabled": "true"
}
```

### Adjust Scroll Speed

```json
{ "FIntScrollWheelDeltaAmount": "140" }
```

### Capture Posts

> [!NOTE]  
> Twitter x Roblox edition.

```json
{ "FFlagCapturesPostEnabledForAll_v4": "true" }
```

### Custom MicroProfiler Scale

```json
{ "DFIntMicroProfilerDpiScaleOverride": "100" }
```

## UI

### Custom Disconnect Message

```json
{
  "FFlagReconnectDisabled": "true",
  "FStringReconnectDisabledReason": "You're stupid and I hate you"
}
```

### Verified Badge

```json
{ "FStringWhitelistVerifiedUserId": "UserID" }
```

### Verified Badge on Everyone

```json
{ "FFlagOverridePlayerVerifiedBadge": "true" }
```

### Display FPS

```json
{ "FFlagDebugDisplayFPS": "true" }
```

### Applies Rainbow Colors to Stuff

```json
{ "FFlagDebugDisplayUnthemedInstances": "true" }
```

### Revert New Invite Menu

```json
{ "FFlagEnableNewInviteMenuIXP2": "false" }
```

### Remove Disconnect Blur/Loading Blur

```json
{ "FIntRobloxGuiBlurIntensity": "0" }
```

### Disable New Chat Translation Settings

```json
{ "FFlagChatTranslationSettingEnabled3": "false" }
```

### Enable New Camera Mode

```json
{ "FFlagNewCameraControls": "true" }
```

### Disable CTM Climbing

```json
{ "FFlagUserClickToMoveSupportAgentCanClimb2": "false" }
```

### Disable Feedback Button in ESC

```json
{ "FFlagDisableFeedbackSoothsayerCheck": "false" }
```

### Disable Camera & Selfview

```json
{ "FFlagSelfieViewEnabled": "true" }
```

### Preferred Text Size Scale

```json
{
  "FFlagEnablePreferredTextSizeGuiService": "true",
  "FFlagEnablePreferredTextSizeScale": "true",
  "FFlagEnablePreferredTextSizeSettingInMenus2": "true"
}
```

### Disable Better Haptics

```json
{ "FFlagEnableBetterHapticsResultHandling": "false" }
```

### New Report Menu

```json
{ "FStringSelectInSceneReportMenuOverrideUserIds": "UserID" }
```

### Removes the Experience Language Option in Settings

```json
{ "FIntV1MenuLanguageSelectionFeaturePerMillageRollout": "0" }
```

### Remove VC Beta Badge

```json
{
  "FFlagVoiceBetaBadge": "false",
  "FFlagTopBarUseNewBadge": "false",
  "FFlagBetaBadgeLearnMoreLinkFormview": "false",
  "FFlagControlBetaBadgeWithGuac": "false",
  "FStringVoiceBetaBadgeLearnMoreLink": "null"
}
```

### VR Controller Transparency

```json
{ "FIntVRTouchControllerTransparency": "0" }
```

### Disable VR Collision Fade

```json
{ "FFlagViewCollisionFadeToBlackInVR": "false" }
```

### Limit Videos Playing

```json
{ "DFIntVideoMaxNumberOfVideosPlaying": "0" }
```

### Disable DSA Reporting In-Game

```json
{ "FFlagDSAIllegalContentReporting2": "false" }
```

### Desktop App Dev Tools ❗

> [!WARNING]  
> Only works on web view windows like profiles, ctrl + shift + I.

```json
{ "FFlagDebugEnableNewWebView2DevTool": "true" }
```

### Show All Error Strings ❗

```json
{ "FFlagDebugEnableErrorStringTesting": "true" }
```

### Customize Chat Translation Settings

```json
{ "FStringChatTranslationEnabledLocales": "es_es,fr_fr,pt_br,de_de,it_it,ja_jp,ko_kr,id_id,tr_tr,zh_cn,zh_tw,th_th,pl_pl,vi_vn,ru_ru," }
```

### Remove the VR Toggle

```json
{ "FFlagAlwaysShowVRToggleV3": "false" }
```

### Mini Webview

```json
{ "FFlagWebViewProtocol": "false" }
```

### Remove Parental Controls Tab

```json
{ "FFlagLuaAppsEnableParentalControlsTab": "false" }
```

### Disable Profile Picture Customization

```json
{ "FFlagAXDefaultAvatarToShopEnabled3": "false" }
```

### Old LuaApp Chat Button

```json
{ "FStringNewChatTabExperimentLayerValue": "2024MUSIC" }
```

### Disable Toast Notifications

```json
{ "FFlagToastNotificationsProtocolEnabled2": "false" }
```

### Cleaner Desktop Home Page

```json
{ "FIntGameGridFlexFeedItemTileNumPerFeed": "0" }
```

### Disable Take A Screenshot of This

```json
{ "FFlagTakeAScreenshotOfThis": "false" }
```

### Do Not Trace Ping

```json
{
  "DFFlagDataPingTrace": "false",
  "DFFlagRakNetPingTrace": "false"
}
```

### Max Delay for Layout Updates

> [!NOTE]  
> Basically the things that are changing on a UI, for example, loading a new page.

```json
{ "DFIntMaxAcceptableUpdateDelay": "15" }
```

### User Interface/Visuals Experimental

#### Draggable Capture Button

```json
{ "FFlagEnableUpdatedCaptureControls_v9": "true" }
```

#### Network Menu Update Rate

> [!NOTE]  
> This fast flag configures how often the network stats menu (Shift + F3) updates its information. By default, it refreshes the information every 1 second. If the value is set to max negative (-2147483647), the information is updated very quickly.

```json
{ "FIntNetworkStatRefreshRate": "1" }
```

#### Disable Centered Experience Details Page

```json
{ "FFlagLuaAppEdpSingleColumnIxp": "false" }
```

#### Don’t Delay Surface App

```json
{ "FFlagPerformanceControlDelaySingleSurfaceAppInit": "false" }
```

#### No More Homepage/Infinite Scrolling

> [!NOTE]  
> Default = 30

```json
{ "FIntTooltipHitboxMinSize": "2147483647" }
```

#### No Opacity to Chrome UI

```json
{ "FFlagChromeUsePreferredTransparency": "false" }
```

#### Multi Try On

> [!NOTE]  
> Allows you to try on multiple things in the catalog and buy everything at once.

```json
{ "FFlagAXEnableMultiTryOnUI": "true" }
```

#### Break Collectible Icon

```json
{ "FFlagDisplayCollectiblesIcon": "false" }
```

#### Changes Some Tiny Things About Party

```json
{ "FFlagAppChatAddConnectUnibarForActiveSquad": "false" }
```

#### Renames Party Back to Roblox Chat

```json
{ "FFlagAppChatRebrandStringUpdates": "false" }
```

#### Disable Sidebar Text (Default: True)

```json
{ "FFlagEnableNavBarLabels3": "false" }
```

#### Hide Playerlist Close Button on Chrome UI

```json
{ "FFlagDisablePlayerListDisplayCloseBtn": "true" }
```

#### Red Font

> [!NOTE]  
> You need to use Default Roblox Font to activate this. Also, it can be glitchy in the settings menu.

```json
{ "FStringDebugHighlightSpecificFont": "rbxasset://fonts/families/BuilderSans.json" }
```

#### ps-ps (Pseudolocalisation)

```json
{
  "FFlagDebugEnablePseudolocalization": "true",
  "FFlagDebugEnableCoreScriptPseudolocalization": "true"
}
```

#### Change How Much Letters In Text

> [!NOTE]  
> This fastflag basically spams every other letter on ROBLOX CoreGUI and the game's GUI but it doesn't affect some parts of the games.  
> Default Value: [7]

```json
{ "FIntDebugTextElongationFactor": "999999" }
```

## Audio

### Uncap Sound Limit

```json
{ "DFIntDebugAudioMaxDecibels": "2147483647" }
```

### Enable Fmod Threading

```json
{ "FFlagFmodUseRuntimeThreading4": "true" }
```

### Voice Chat Range/Volume

> [!NOTE]  
> For people that play Roblox on low volume, 10000 is the optimal range/volume, but it’s a personal opinion, so adjust it to your liking, and I hope this flag is useful.

```json
{ "DFIntVoiceChatVolumeThousandths": "10000" }
```

### Allows You to Change Voice Chat Distance

> [!NOTE]  
> Default: [Min 7 Max 80]

```json
{
  "DFIntVoiceChatRollOffMinDistance": "7",
  "DFIntVoiceChatRollOffMaxDistance": "80"
}
```

### Sounds Use Physical Velocity and Become Distorted

> [!NOTE]  
> <2017 but still works.

```json
{ "FFlagSoundsUsePhysicalVelocity": "true" }
```

### Audio Occlusion

```json
{ "FFlagDebugEnableDirectAudioOcclusion2": "true" }
```

### Limit Audios That Are Being Played

```json
{ "DFIntMaxLoadableAudioChannelCount": "1" }
```

### Mess With Voice Chat Volume

> [!NOTE]  
> Default = 1000

```json
{ "DFIntVoiceChatVolumeThousandths": "100000" }
```

### No Sounds

```json
{ "FFlagDebugRomarkMockingAudioDevices": "true" }
```

## Latency

### Fix Layered Clothing

> [!NOTE]  
> https://devforum-uploads.s3.dualstack.us-east-2.amazonaws.com/uploads/original/5X/f/a/5/7/fa576e1b777534a50b0859e2b75e5ad6872dee47.gif

```json
{
  "FIntRigidityOuterLayerWeightPct": "45",
  "FIntOuterCageResOver100": "22",
  "FFlagWrappedGridFixCLI148409": "true",
  "FFlagUseBothCagesForRBFDeformer": "true",
  "FFlagMergeBodyCageByR15Connectivity": "true",
  "FFlagEnableLinearCageDeformer2": "true",
  "FFlagRigidityControl": "true",
  "FFlagCheckDuplicateCagePoints": "true"
}
```

### Network Ownership

> [!NOTE]  
> https://create.roblox.com/docs/physics/network-ownership

```json
{
  "DFIntMinClientSimulationRadius": "2147000000",
  "DFIntMinimalSimRadiusBuffer": "2147000000",
  "DFIntMaxClientSimulationRadius": "2147000000",
  "DFFlagDebugPhysicsSenderDoesNotShrinkSimRadius": "true",
  "FFlagDebugUseCustomSimRadius": "true"
}
```

### SERVER LOCATION OPTIMIZE

> [!WARNING]  
> If you don’t know everything, don’t use it.  
> Default = 100

```json
{ "DFIntTrackCountryRegionAPIHundredthsPercent": "10000" }
```

### Disable Walk Speed Scale Based

```json
{ "DFFlagUserAnimateScaleRun": "false" }
```

### Enable SmoothInputOffset

> [!NOTE]  
> "Smooth Input Offset" helps deliberately slow down or filter input signals, making mouse or controller movements smoother and preventing sudden stuttering or jittering.  
> The game smooths out the movement by averaging or slightly delaying the input, creating a more fluid control experience — even if it means sacrificing a bit of precision or immediate responsiveness.

```json
{ "FFlagSmoothInputOffset": "true" }
```

### Faster Precise Time

> [!NOTE]  
> Faster response: Helps actions like jumping, shooting, or moving become more precise and instantaneous.  
> Smoother visual effects: Effects like lighting and physics-based movements are updated more accurately in real time.

```json
{ "FFlagFasterPreciseTime4": "true" }
```

### Enable CoalesceInput (Smooth Multi Responsive)

> [!NOTE]  
> A feature or input processing technique that combines multiple control signals into a smoother and faster-responding experience. It is commonly used to improve sensitivity and accuracy when players interact with the game using a keyboard, mouse, controller, or touch input.

```json
{ "FFlagCoalesceInput": "true" }
```

### Preferred Input (Prioritize Input)

> [!NOTE]  
> https://devforum.roblox.com/t/client-beta-introducing-preferredinput-and-improved-touch-capabilities/3750890/1

```json
{ "FFlagPreferredInput": "true" }
```

### Keyboard, Mouse, Gamepad, Touch Latency

> [!NOTE]  
> Default value: 500 >> Lower value = more responsive.

```json
{
  "FIntActivatedCountTimerMSKeyboard": "0",
  "FIntActivatedCountTimerMSMouse": "0",
  "FIntActivatedCountTimerMSGamepad": "0",
  "FIntActivatedCountTimerMSTouch": "0"
}
```

### Zero Delay With Mouse

> [!NOTE]  
> Default value: 16 >> Lower value = more double click.

```json
{ "FIntCLI20390_2": "0" }
```

### Better Serversided Character Position

> [!NOTE]  
> 100 makes your serversided character closer to your client.

```json
{ "DFIntS2PhysicsSenderRate": "100" }
```

### Stop Shrinking Simulation Radius

> [!NOTE]  
> Normally, DFIntS2PhysicsSenderRate controls how much physical data is being sent and increases synchronization with the server, but the simulation radius (the area around you where physics are actively processed) gets reduced over time.  
> Enabling this flag stops that shrinking behavior, meaning the simulation radius stays large and consistent.  
> This helps keep physics interactions responsive across a wider area around your character, especially useful in games with vehicles or moving parts that go beyond the default radius.

```json
{ "DFFlagDebugPhysicsSenderDoesNotShrinkSimRadius": "true" }
```

### Dev Console Logging

> [!NOTE]  
> Changes how long a Message can be, doesn't give you the ability to exceed the 16k Message Length Limit.

```json
{ "FIntStandardOutputMaximumCharacterLength": "1" }
```

### Dev Console Log Count

> [!NOTE]  
> Control how many developer console logs can be shown at once, for example, if you set the limit to be 100, then 100 different log messages will be shown while any older ones will be deleted when the limit is reached.

```json
{ "FIntNewDevConsoleMaxLogCount": "2" }
```

### Replace All Decals With a Test Image

```json
{ "FFlagDebugTestImageDrawItem": "true" }
```

### Allows You to Edit the DataModel Patch ❗

> [!WARNING]  
> You can get banned by Roblox for modifying. Risk by yourself.

```json
{ "FFlagDataModelPatcherForceLocal": "true" }
```

### Shows the State of a Flag

```json
{ "FStringDebugShowFlagState": "FLAG_HERE" }
```

> [!TIP]  
> ```json
> { "FStringDebugShowFlagState": "DFIntTaskSchedulerTargetFps, ChannelName" }
> ```
