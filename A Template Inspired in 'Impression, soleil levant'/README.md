# Impression Template Documentation

This template was created based on the painting "Impression, soleil levant" by Claude Monet (1872). Some basic information should be clarified for better use.

First, the compiler I used is XeLaTeX (it’s probably possible to use LuaLaTeX as well, but I don’t think it’s necessary). The main reason for using this compiler was that I wanted to use the **EB Garamond** font with some extra options, which required the `fontspec` package. As a result, the file takes a bit longer to compile, and consequently, larger files may exceed Overleaf’s compilation time limit. Therefore, I strongly recommend that if you plan to use this template for extensive writing, you use it locally (e.g., in VSCode), as this way there will be no compilation time limit.

There are 7 custom colors in this template, 5 of which, when combined, form the color palette of the painting. If you want to use any of them, they are:
- MyGray
- MyLightGray
- MyLightBlue
- MyDarkBlue
- MyOrange

In addition to the painting’s palette, there are MyWhite, which is the base color of the pages, and MyBlack, which is the main text color. All of them are defined starting from line 21 of the `impression.cls` file.

If you liked the template and want to use a different artwork, I’ll explain how to do it. Before swapping the image, you need to adjust the new artwork to have proportions similar to the painting I used, which is 48 x 63 (in pixels, it’s 1601 x 1243). Once that’s done, upload the image to the `Figures` folder, go to the `impression.cls` file, and replace all instances of "Figures/Impression, soleil levant - Claude Monet.png" with "Figures/Your Image Name.png" (using Ctrl + F makes it easier).

On the content pages, there’s a vanilla flower that I found very beautiful and wanted to include in the template. But if you don’t like it `D:`, you can simply delete line 85 of the `impression.cls` file.

All packages were placed in a separate file (`mypackages.sty`) for better organization, so I recommend adding more packages to this file. However, this is just for organization—you can add packages to either `main.tex` or `impression.cls`, and it won’t make any difference.

If you are going to write your texts in Portuguese, go to the `mypackages.sty` file and change `\RequirePackage[english]{babel}` to `\RequirePackage[brazilian]{babel}` (line 19).

That’s it! The template isn’t perfect, it has my workarounds, but it works nicely, hehe.
