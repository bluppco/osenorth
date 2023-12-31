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
- JS network calls. - Not calling any JS module.

        Currently - 7 calls, 112Kb.
        Updated - 0 calls, 0Kb.
  
- Images network calls - **279% better**

        Currently - 14 calls, 9.61Mb.
        Updated - 20 calls, 2.53Mb.
  
- HTML network calls - **170% better**

        Currently - 73.33Kb.
        Updated - 27.14Kb. 
  
- CSS network calls - **64% better**.

        Currently - 2 calls, 23.4Kb.
        Updated - 1 call, 14.23Kb. 

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
