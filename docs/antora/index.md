# Install


Include
https://gitlab.com/antora/antora/-/issues/596

## Antora process
1. Convert docx to html
pandoc -f docx -t html -s -o PMM.html PMM.docx

2. Clean html

3. Convert html to md
pandoc -s -r html pmm.html -o pmm.md

4. Convert md to ascii
Webpage to docx
pandoc --reference-doc pandocTheme.docx -f html -t docx -o HugiOmg.docx http://127.0.0.1:5000/ess/performance-management/index.html#_plan_assignment
wkhtmltopdf http://127.0.0.1:4000/docs/CSharpCodingStandards.html google.pdf


## Conversion
pip3 uninstall mkpdfs-mkdocs


## Serve
1. Install
npm i -g http-server
yarn global add http-server




npm i -g @asciidoctor/core asciidoctor-pdf
npm run clean-install and then npm run build

 
gem install asciidoctor
 
## Misc
npm i -g @asciidoctor/core asciidoctor-pdf
npm run clean-install and then npm run build