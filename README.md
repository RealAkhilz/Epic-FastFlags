> [!important]
> https://discord.gg/848BdgmvD9

<h1 align="center">FastFlags Lab</h1>

<h3 align="center"> Made by <a href="https://guns.lol/realakhil">RealAkhilz</a> </h3>

- - -

<h2>🚀 Quick Links </h2>

<div align="center">

[![guns.lol](https://img.shields.io/badge/guns.lol-RealAkhilz-darkblue?style=flat&logo=link&logoColor=white)](https://guns.lol/realakhil)
[![Discord](https://img.shields.io/discord/1380077621974667264?label=Discord&color=5865F2&logo=discord&logoColor=white)](https://discord.gg/848BdgmvD9)

</div>

- - -

<h2>🏴 FastFlags </h2>

> [!Important]
> Some fastflags have !Important, !Warning, and !Caution, please read the fastflags that have these and use fastflags wisely.

<h2 align="center"> Rendering API </h2>

<h3>Direct3D 11</h3>

```json
{ "FFlagDebugGraphicsPreferD3D11": "True" }
```

<h3>Direct3D 10</h3>

```json
{ "FFlagDebugGraphicsPreferD3D11FL10": "True" }
```

<h3>Metal</h3>

> [!note]
> This rendering API is only for MacOS

```json
{ "FFlagDebugGraphicsPreferMetal": "True" }
```

<h3>Vulkan</h3>

```json
{ "FFlagDebugGraphicsDisableDirect3D11": "True", "FFlagDebugGraphicsPreferVulkan": "True" }
```

<h3>OpenGL</h3>

```json
{ "FFlagDebugGraphicsDisableDirect3D11": "True", "FFlagDebugGraphicsPreferOpenGL": "True" }
```

<h2 align="center">Graphic and Rendering FastFlags</h2>

<h3>Kilo Pixels</h3>

> [!note]
> This fastflag changes Roblox resolution in kilo pixels, like the youtube graphics slider (Roblox GUI and game UI unaffected)

<pre>
4320p (8k) - 33178
2160p (4k) - 8294
1440p (2K) - 3686
1080p (FHD) - 2074
720p (HD) - 922
480p (SD) - 410
360p (Low SD) - 230
</pre>

```json
{ "DFIntDebugDynamicRenderKiloPixels": "-1" }
```

<h3>Minimal Rendering</h3>

> [!note]
> Renders certain terrain and textures at a lower quality, potentially improving performance

```json
{ "FFlagDebugRenderingSetDeterministic": "True" }
```
