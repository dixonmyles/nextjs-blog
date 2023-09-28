---
title: 'Image Optimization with Next.JS'
date: '2023-09-28'
---

Next.js supports out of the box Image Optimization through the **next/image** component, **Image**.

By using the Image component instead of a standard **<img>** tag, you get the following optimization features out-of-the-box:

- Conversion to modern web formats such as webp and avif
- Automatically send smaller images based on screen size
  - desktop: 464KB image
  - mobile: 70 KB image
- Next.js automatically configures default breakpoints for your images
  - [640, 750, 828, 1080, 1200, 1920, 2048, 3840]
- Next.js accounts for image position to reduce Cumulative Layout Shift

Additionally, Next.js will automatically lazy load your images. This means that your images will not be fetched from the server while they are out of frame, saving network traffic and increasing performance. As a user begins to scroll towards the image, the image will begin to be loaded and become available once its container element is in view.