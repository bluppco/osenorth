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
- Delivering images and videos via CDN.
- Adding 40% opacity of black color for the text to be prominent on the masthead video.
- JS network calls. Currently - 345Kb; Updated - 0Kb; Better - Infintely better. Not calling any JS module.
- Images network calls. Currently - 9.62Mb; Updated - 1.65Mb. **483% better**.
- HTML network calls. Currently - 77.33Kb; Updated - 11.07Kb. **598% better**.
- CSS network calls. Currently - 23.4Kb; Updated - 22.45Kb. **4% better**.

## Things not touched
- I could optimised the images further by requesting sized images from the browser, i.e. if request is coming from mobile, request half the resolution of image. Say, not a 1500x1000 image but instead 750x500. Tradeoff of writing JS vs reducing image size.

## Technology
- Astro
- Tailwind
- BunnyCDN
- Cloudflare

## How to run the project
- Clone the project.
- install packages

        npm i
- run astro project

        npm run dev
- Enjoy
