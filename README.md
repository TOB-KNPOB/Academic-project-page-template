# Paper page template

This is an academic paper project page template. Example project pages built using this template are:

- https://www.vision.huji.ac.il/deepsim/
- https://www.vision.huji.ac.il/3d_ads/
- https://www.vision.huji.ac.il/ssrl_ad/
- https://www.vision.huji.ac.il/conffusion/
- https://liu-qilong.github.io/udmc/

## Start using the template

To start using the template, click on `Use this Template`. If you have already created a code repository for your project, you can copy the `.github/`, `static/`, and `index.html` folders and files to the root directory of your project repository. GitHub Pages will be built after you push changes to your `main` branch, and the building process and link can be checked under the `Actions` tab on your repository's GitHub main page.

_P.S. If the main branch of your repository is `master`, please edit the 7th line of `.github/workflows/static.yml` accordingly._

The template uses html for controlling the content and css for controlling the style. 
To edit the websites contents edit the `index.html` file. It contains different HTML "building blocks", use whichever ones you need and comment out the rest.  

**IMPORTANT!** Make sure to replace the `favicon.ico` under `static/images/` with one of your own, otherwise your favicon is going to be a dreambooth image of me.

## Components

- Multiple columns layout

    _P.S. Useful for comparing the results of your approach with previous works._

- Teaser video/image
- Youtube video embedding
- Images Carousel
- Video Carousel
- PDF Poster
- BibTex citation

## Tips:

- The `index.html` file contains comments instructing you what to replace, you should follow these comments.
- The `meta` tags in the `index.html` file are used to provide metadata about your paper 
(e.g. helping search engine index the website, showing a preview image when sharing the website, etc.)
- The resolution of images and videos can usually be around 1920-2048, there rarely a need for better resolution that take longer to load. 
- All the images and videos you use should be compressed to allow for fast loading of the website (and thus better indexing by search engines). For images, you can use [TinyPNG](https://tinypng.com), for videos you can need to find the tradeoff between size and quality.

> Resizing video to half-width and half-height with `ffmpeg`:
> ```
> $ ffmpeg -i source.mp4 -vf scale="iw*0.5:ih*0.5" output.mp4
> ```
>  Resizing image to half-width and half-height with `convert`:
> ```
> $ convert -resize 50% source.png output.jpg
> ```

- When using large video files (larger than 10MB), it's better to use youtube for hosting the video as serving the video from the website can take time.
- Using a tracker can help you analyze the traffic and see where users came from. [statcounter](https://statcounter.com) is a free, easy to use tracker that takes under 5 minutes to set up. 
- This project page can also be made into a github pages website.
- Replace the favicon to one of your choosing. 
- Suggestions, improvements and comments are welcome, simply open an issue or contact me. You may also contact the original author with contact information at [https://pages.cs.huji.ac.il/eliahu-horwitz/](https://pages.cs.huji.ac.il/eliahu-horwitz/)

## Acknowledgments

Parts of this project page were adopted [Academic Project Page Template](https://github.com/eliahuhorwitz/Academic-project-page-template) from the [Nerfies](https://nerfies.github.io/) page.

## Website License

[![Creative Commons License](https://i.creativecommons.org/l/by-sa/4.0/88x31.png)](http://creativecommons.org/licenses/by-sa/4.0/)

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/).
