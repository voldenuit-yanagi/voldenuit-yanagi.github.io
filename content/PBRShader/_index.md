---
title: PBR Shader
description: xxxxxxx
featured_image: janis-ringli-UC1pzyJFyvs-unsplash.jpg
weight: 1

# list pages require at least one image to be displayed.
---

## Microfacet Model and Image-based Lighting
xxxx

图片及图片文字说明


## Real-time Shadows
implemented Two Pass Shadow Map for hard shadows; implement PCF (Percentage Closer Filter) and PCSS (Percentage Closer Soft Shadow) for soft shadows.

图片及图片文字说明 图片及图片文字说明
图片及图片文字说明


## Real-time Environment Mapping
implemented PRT (Precomputed Radiance Transfer), including fitting three kinds of lighting and light transport with spherical harmonics in the offline path tracing toolchain, as well as using the precomputed coefficients in the WebGL framework.

图片及图片文字说明 图片及图片文字说明


## Real-time Global Illumination
first calculated direct lighting, then implemented Screen Space Ray Tracing (SSR) to find the radiance of the second ray, and finally solved the rendering equation for the indirect lighting using the Monte Carlo method.

图片及图片文字说明 图片及图片文字说明


## Physically Based Materials
used Kulla-Conty BRDF to make up the energy loss of Microfacet BRDF, including off-line computing the two prior variables and real-time calculating the energy compensation term.

图片及图片文字说明 图片及图片文字说明


## Real-time Ray Tracing
implemented denoising for simple real-time ray tracing, including single frame denoising, motion vector calculation, and temporal accumulation.

视频及视频文字说明 视频及视频文字说明