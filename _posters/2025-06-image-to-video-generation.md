---
title: "Image-to-Video Generation Using Diffusion Models"
collection: posters
type: "Poster Presentation"
permalink: /posters/2025-06-image-to-video-generation
venue: "MSc AI Research Showcase, Lab42"
date: 2025-06-01
location: "University of Amsterdam, Amsterdam, The Netherlands"
posterurl: '/files/Image-to-Video-Generation-Poster.pdf'
excerpt: 'Explored generating interior video tours from single high-resolution images using diffusion-based video models. Evaluated post-processing pipelines achieving SSIM up to 0.917.'
---

## Abstract

This poster presents research on generating interior video tours from single high-resolution images using diffusion-based video generation models. The work addresses the challenge of creating smooth, realistic video sequences from static images, with applications in virtual tours, architectural visualization, and content creation.

## Methodology

We evaluated various post-processing pipelines (denoising, upscaling, and their combinations) on 18 generated videos using quantitative metrics including Peak Signal-to-Noise Ratio (PSNR) and Structural Similarity Index (SSIM). The research systematically compared different pipeline orderings to understand their impact on perceptual quality.

## Key Findings

Our evaluation revealed that the order of post-processing operations significantly impacts output quality. Specifically, we found that **denoising→upscaling** versus **upscaling→denoising** leads to substantial differences in perceptual quality, with SSIM values reaching up to **0.917** for optimal pipeline configurations.

This finding highlights the importance of carefully designing post-processing workflows for diffusion-based video generation, as the sequence of operations can dramatically affect the final visual quality of generated content.

## Team

**Konstantinos Zafeirakis**, Elyanne X, Lisanne X, Taiki X, Wojciech X

## Download

[Download Poster PDF](/files/Image-to-Video-Generation-Poster.pdf)

