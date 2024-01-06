---
title: OpenGL Shaders
description: xxxxxxx
featured_image: https://aliyun-image-host.oss-cn-hongkong.aliyuncs.com/2023-12-12-PCSS.png
weight: 3

# list pages require at least one image to be displayed.
---

## Microfacet Model and Image-based Lighting
xxxx

一行两个


<div class="columns-2">
<div> <img class=" w-full aspect-video" src="https://aliyun-image-host.oss-cn-hongkong.aliyuncs.com/2023-12-14-Microfacet-BRDF-IBL.gif" ></img>
<div style="text-align:center">这是一个简单备注 </div>
</div>
<div><img class=" w-full  aspect-video" src="https://aliyun-image-host.oss-cn-hongkong.aliyuncs.com/2023-12-14-Disney-BRDF-IBL.gif"> </img> </div>
<div style="text-align:center">这是一个简单备注 </div>



</div>





## Real-time Shadows
<hr class="h-px  bg-gray-200 border-0 dark:bg-gray-700"  />
implemented Two Pass Shadow Map for hard shadows; implement PCF (Percentage Closer Filter) and PCSS (Percentage Closer Soft Shadow) for soft shadows.

图片分两列

<img class="h-10 w-10 " src="https://aliyun-image-host.oss-cn-hongkong.aliyuncs.com/2023-12-12-ShadowMap.png" /> 

<img class="h-10 w-10 " src="https://aliyun-image-host.oss-cn-hongkong.aliyuncs.com/2023-12-12-PCF.png" /> 

<img class="h-10 w-10 " src="https://aliyun-image-host.oss-cn-hongkong.aliyuncs.com/2023-12-12-PCSS.png" /> 


说明文字放在对应图片的下面

## Real-time Environment Mapping
implemented PRT (Precomputed Radiance Transfer), including fitting three kinds of lighting and light transport with spherical harmonics in the offline path tracing toolchain, as well as using the precomputed coefficients in the WebGL framework.

图片分两列
<img class="h-10 w-10 rounded-full" src="https://aliyun-image-host.oss-cn-hongkong.aliyuncs.com/2023-12-12-Diffuse%20Shadowed.png" style="max-with:100%" /> 



<img class="h-10 w-10 rounded-full" src="https://aliyun-image-host.oss-cn-hongkong.aliyuncs.com/2023-12-12-Diffuse%20Inter-reflection.png" style="max-with:100%" /> 

说明文字放在对应图片的下面

## Real-time Global Illumination
first calculated direct lighting, then implemented Screen Space Ray Tracing (SSR) to find the radiance of the second ray, and finally solved the rendering equation for the indirect lighting using the Monte Carlo method.

图片分两列

<img class="h-10 w-10 rounded-full" src="https://aliyun-image-host.oss-cn-hongkong.aliyuncs.com/2023-12-12-cube.png"  /> 



说明文字放在对应图片的下面

## Physically Based Materials
used Kulla-Conty BRDF to make up the energy loss of Microfacet BRDF, including off-line computing the two prior variables and real-time calculating the energy compensation term.

图片分两列

<img class="h-10 w-10 rounded-full" src="https://aliyun-image-host.oss-cn-hongkong.aliyuncs.com/2023-12-12-KullaConty.png"  /> 


<img class="h-10 w-10 rounded-full" src="https://aliyun-image-host.oss-cn-hongkong.aliyuncs.com/2023-12-12-KullaContywithIBL.png"  /> 

说明文字放在对应图片的下面

## Real-time Ray Tracing
implemented denoising for simple real-time ray tracing, including single frame denoising, motion vector calculation, and temporal accumulation.

一行两个

<img class="h-10 w-10 rounded-full" src="https://aliyun-image-host.oss-cn-hongkong.aliyuncs.com/2023-12-14-box-input.gif"  /> 

<img class="h-10 w-10 rounded-full" src="https://aliyun-image-host.oss-cn-hongkong.aliyuncs.com/2023-12-14-box-result.gif"  /> 

说明文字放在对应动图的下面
