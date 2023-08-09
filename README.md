# osenorth
An award winning full-service creative agency, infinitely crazy about functional, emotional and polished digital interfaces and products.

## Problems
- Images and Videos taking too much time to load.
- Videos not loading on iPhone and iPad. Tested all the browsers but did not work.
- Missing metatags.
- Missing robots.txt file.
- Missing sitemap.xml file.

## Changes
- Webm file format for video doesn't work on iPhone browsers. I converted it to mp4 so that it could be played on all the devices.
- Delivering images and videos via CDN. Vercel is nice but they are not good with deliverying assets. Plus the cost of images optimised by them is too high as compared to other options available.
- Adding 40% opacity of black color for the text to be prominent on the masthead video.
- JS network calls.
        Currently - 7 calls, 112Kb.
        Updated - 0 calls, 0Kb. Better - Infintely better. Not calling any JS module.
- Images network calls.
        Currently - 26 calls, 18.7Mb.
        Updated - 21 calls, 2.56Mb. **630% better**.
- HTML network calls.
        Currently - 17.89Kb;
        Updated - 5.72Kb. **212% better**.
- CSS network calls.
        Currently - 2 calls, 5.5Kb.
        Updated - 1 call, 4.1Kb. **34% better**.

## Things not touched
- I could optimised the images further by requesting sized images from the browser, i.e. if request is coming from mobile, request half the resolution of image. Say, not a 1500x1000 image but instead 750x500. Tradeoff of writing JS vs reducing image size.

## Technology
- Astro
- Tailwind
- CDN
- Cloudflare

## Font
- IBM Plex Sans - available for free.

## How to run the project
- Clone the project.
- install packages

        npm i
- run astro project

        npm run dev
- Enjoy 🎉
