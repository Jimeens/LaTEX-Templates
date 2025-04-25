# [PT/BR] Documentação do Template

Este template foi criado baseado na pintura "Impression, soleil levant" do Claude Monet (1872). Algumas informações básicas devem ser deixadas mais claras para melhor uso.

Em primeiro lugar, o compilador que eu utilizei é o XeLaTeX (provavelmente seja possível utilizar LuaLaTeX também, porém não acho necessário). O principal motivo de usar este compilador foi o fato de que eu queria utilizar a fonte **EB Garamond** com algumas opções extras e para isso era necessário utilizar o pacote `fontspec`, portanto o arquivo demora um pouco mais para compilar e consequentemente arquivos maiores devem ultrapassar o limite de compilação do Overleaf, de modo que eu recomendo fortemente que caso você queira utilizar esse template para escrever bastante, utilize ele localmente (VScode, etc), pois dessa forma não vai ter limite de tempo de compilação.

Existem 7 cores personalizadas nesse template, em que 5 delas, quando juntas, formam a paleta de cor da pintura, então caso você queira utilizar alguma, elas são:MyGray
- MyLightGray
- MyLightBlue
- MyDarkBlue
- MyOrange

Além da paleta do quadro, tem o MyWhite, que é a cor base das páginas e MyBlack, que é a cor principal do texto. Todas elas estão definidas a partir da linha 21 do arquivo `impression.cls`.

Caso você tenha gostado do template e queira utilizar alguma outra arte, vou ensinar a fazer. Antes de trocar a imagem, você precisa deixar a arte nova com dimensões proporcionais à da pintura q eu utilizei, que é de 48 x 63 (em pixels ficou com 1601 x 1243), feito isso você faz upload da imagem dentro da pasta `Figures`, vai no arquivo `impression.cls` e substitui todos os `"Figures/Impression, soleil levant - Claude Monet.png"` para `"Figures/Nome da sua Imagem.png"` (usa o ctrl + F que fica mais fácil).

Nas páginas de conteúdo, tem uma flor de baunilha que eu achei muito bonita e quis colocar no template, mas se você não gosta dela `D:` é só excluir a linha 85 do arquivo `impression.cls`.

Todos os pacotes foram colocados em um arquivo separado (`mypackages.sty`) pra ficar mais organizado, então recomendo colocar mais pacotes nesse arquivo, mas é apenas pra organização, você pode colocar tanto no `main.tex` quanto no `impression.cls` que não vai mudar nada.

É isso, o template não é perfeito, tem minhas gambiarras, mas funciona bonitinho. Qualquer coisa, lcsximenes@usp.br.



# [EN] Template Documentation

This template was created based on the painting "Impression, soleil levant" by Claude Monet (1872). Some basic information should be clarified for better use.

First, the compiler I used is XeLaTeX (it’s probably possible to use LuaLaTeX as well, but I don’t think it’s necessary). The main reason for using this compiler was that I wanted to use the **EB Garamond** font with some extra options, which required the `fontspec` package. As a result, the file takes a bit longer to compile, and consequently, larger files may exceed Overleaf’s compilation time limit. Therefore, I strongly recommend that if you plan to use this template for extensive writing, you use it locally (e.g., in VSCode), as this way there will be no compilation time limit.

There are 7 custom colors in this template, 5 of which, when combined, form the color palette of the painting. If you want to use any of them, they are:
- MyGray
- MyLightGray
- MyLightBlue
- MyDarkBlue
- MyOrange

In addition to the painting’s palette, there are MyWhite, which is the base color of the pages, and MyBlack, which is the main text color. All of them are defined starting from line 21 of the `impression.cls` file.

If you liked the template and want to use a different artwork, I’ll explain how to do it. Before swapping the image, you need to adjust the new artwork to have proportions similar to the painting I used, which is 48 x 63 (in pixels, it’s 1601 x 1243). Once that’s done, upload the image to the `Figures` folder, go to the `impression.cls` file, and replace all instances of `"Figures/Impression, soleil levant - Claude Monet.png"` with `"Figures/Your Image Name.png"` (using Ctrl + F makes it easier).

On the content pages, there’s a vanilla flower that I found very beautiful and wanted to include in the template. But if you don’t like it `D:`, you can simply delete line 85 of the `impression.cls` file.

All packages were placed in a separate file (`mypackages.sty`) for better organization, so I recommend adding more packages to this file. However, this is just for organization—you can add packages to either `main.tex` or `impression.cls`, and it won’t make any difference.

If you are going to write your texts in Portuguese, go to the `mypackages.sty` file and change `\RequirePackage[english]{babel}` to `\RequirePackage[brazilian]{babel}` (line 19).

That’s it! The template isn’t perfect, it has my workarounds, but it works nicely. For support or inquiries, lcsximenes@usp.br.
