# Authoring

Antora authring guidelines
## Include
https://gitlab.com/antora/antora/-/issues/596

## Antora process
1. Do conversion (HTML/DocX/Markdown)
2. Clean html
3. Convert html to md
4. Convert md to ascii

## Conversion

### Docx to Markdown 

Docx to Markdown with images

``` python 
pandoc -o SalaryRegister.md --extract-media=./ SalaryRegister.docx
```

### HTML to Docx
``` bash 
pandoc --reference-doc pandocTheme.docx -f html -t docx -o DailyTS.docx https://site/wagetype-based-timesheet/
```

### HTML to Markdown
pandoc -s -r html pmm.html -o pmm.md


### To ASCIIDOC

``` bash linenums="1"
pandoc -f html -t asciidoctor -o PRL_PayrollSheet00.adoc PRL_PayrollSheet00.html 
```

## Webpage to docx

``` bash
pandoc --reference-doc pandocTheme.docx -f html -t docx -o HugiOmg.docx http://127.0.0.1:5000/ess/index.html
```

``` bash
wkhtmltopdf http://127.0.0.1:4000/docs/CSharpCodingStandards.html google.pdf
```

## Weasyprint

``` bash 
python -m weasyprint http://weasyprint.org weasyprint.pdf
```

# Antora commands

``` python 
antora antora-playbook.yml
antora --fetch antora-playbook.yml
antora --fetch author-mode.yml 
```

``` python 
set "DOCSEARCH_ENABLED=true" && set "DOCSEARCH_ENGINE=lunr" && antora --generator antora-site-generator-lunr antora-playbook.yml
```

``` python 
set "DOCSEARCH_ENABLED=true" && set "DOCSEARCH_ENGINE=lunr" && antora --generator antora-site-generator-lunr author-mode.yml
```

``` python 
http-server build/site -c-1 -p 5000 DDOCSEARCH_ENABLED=true DOCSEARCH_ENGINE=lunr antora site.yml
```

## Local site preview

``` python
set "DOCSEARCH_ENABLED=true" && set "DOCSEARCH_ENGINE=lunr" && antora --generator antora-site-generator-lunr local-playbook.yml
``` 

## Serve
1. Install server

``` python linenums="1"
npm i -g http-server

OR 

yarn global add http-server
``` 

``` python linenums="1"
http-server build/site -c-1
http-server build/site -c-1 -p 5000
-c-1 flag to disable caching
``` 

## Misc
npm i -g @asciidoctor/core asciidoctor-pdf
npm run clean-install and then npm run build


## Formatting


[%autowidth]
|===
| A
| B
| C
|===

## Mindfulness
https://www.youtube.com/watch?v=7-bPYMAdnnM
https://www.youtube.com/watch?v=h-CYAQqpvcw



## Doctype book level 0 error

= Book Title
:chapter: 12
:sectnums: 
:sectnumoffset: 11  (chapter minus 1)
:leveloffset: 1

= Chapter Title 