---
title: OpenGL Shaders
description: xxxxxxx
featured_image: https://aliyun-image-host.oss-cn-hongkong.aliyuncs.com/2023-12-12-PCSS.png
weight: 3

# list pages require at least one image to be displayed.
---

## Surface Model and Image-based Lighting
xxxx

<div class="columns-2">
    <div> 
        <img class="w-full aspect-video" src="https://aliyun-image-host.oss-cn-hongkong.aliyuncs.com/2023-12-14-Microfacet-BRDF-IBL.gif" ></img>
        <div>Microfacet Model and IBL</div>
    </div>
    <div>
        <img class="w-full  aspect-video" src="https://aliyun-image-host.oss-cn-hongkong.aliyuncs.com/2023-12-14-Disney-BRDF-IBL.gif"> </img>
        <div>Disney-BRDF and IBL </div>
    </div>
</div>

## Real-time Shadows
Implemented Two Pass Shadow Map for hard shadows; implement PCF (Percentage Closer Filter) and PCSS (Percentage Closer Soft Shadow) for soft shadows.

<div class="columns-3">
    <div> 
        <img class="w-full" src="https://aliyun-image-host.oss-cn-hongkong.aliyuncs.com/2023-12-12-ShadowMap.png" /> 
        <div>Two Pass Shadow Map</div>
    </div>
    <div>
        <img class="w-full" src="https://aliyun-image-host.oss-cn-hongkong.aliyuncs.com/2023-12-12-PCF.png" /> 
        <div>PCF</div>
    </div>
    <div>
        <img class="w-full" src="https://aliyun-image-host.oss-cn-hongkong.aliyuncs.com/2023-12-12-PCSS.png" /> 
        <div>PCSS</div>
    </div>
</div>

## Real-time Environment Mapping
Implemented PRT (Precomputed Radiance Transfer), including fitting three kinds of lighting and light transport with spherical harmonics in the offline path tracing toolchain, as well as using the precomputed coefficients in the WebGL framework.

<div class="columns-2">
    <div> 
        <img class="w-full" src="https://aliyun-image-host.oss-cn-hongkong.aliyuncs.com/2023-12-12-Diffuse%20Shadowed.png" style="max-with:100%" />
        <div>Shadowed</div>
    </div>
    <div>
        <img class="w-full" src="https://aliyun-image-host.oss-cn-hongkong.aliyuncs.com/2023-12-12-Diffuse%20Inter-reflection.png" style="max-with:100%" />
        <div>Inter-reflection</div>
    </div>
</div>

## Real-time Global Illumination
First calculated direct lighting, then implemented Screen Space Ray Tracing (SSR) to find the radiance of the second ray, and finally solved the rendering equation for the indirect lighting using the Monte Carlo method.

<div class="columns-2">
    <div> 
        <img class="w-full" src="https://aliyun-image-host.oss-cn-hongkong.aliyuncs.com/2023-12-12-cube.png" />
        <div>cube</div>
    </div>
    <div> 
        <img class="w-full" src="https://aliyun-image-host.oss-cn-hongkong.aliyuncs.com/2023-12-12-cave.png" />
        <div>cave</div>
    </div>
</div>


## Physically Based Materials
Used Kulla-Conty BRDF to make up the energy loss of Microfacet BRDF, including off-line computing the two prior variables and real-time calculating the energy compensation term.

<div class="columns-2">
    <div> 
        <img class="w-full" src="https://aliyun-image-host.oss-cn-hongkong.aliyuncs.com/2023-12-12-KullaConty.png" />
        <div>Kulla-Conty</div>
    </div>
    <div> 
        <img class="w-full" src="https://aliyun-image-host.oss-cn-hongkong.aliyuncs.com/2023-12-12-KullaContywithIBL.png" /> 
        <div>Kulla-Conty with IBL</div>
    </div>
</div>

## Real-time Ray Tracing
Implemented denoising for simple real-time ray tracing, including single frame denoising, motion vector calculation, and temporal accumulation.

<div class="columns-2">
    <div> 
        <img class="w-full" src="https://aliyun-image-host.oss-cn-hongkong.aliyuncs.com/2023-12-14-box-input.gif" /> 
        <div>Conell Box Input</div>
    </div>
    <div> 
        <img class="w-full" src="https://aliyun-image-host.oss-cn-hongkong.aliyuncs.com/2023-12-14-box-result.gif" />  
        <div>Conell Box Result</div>
    </div>
</div>
