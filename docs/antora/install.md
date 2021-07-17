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
#Docx to Markdown with Images

pandoc -o SalaryRegister.md --extract-media=./ SalaryRegister.docx

pip3 uninstall mkpdfs-mkdocs

python -m weasyprint http://weasyprint.org weasyprint.pdf


pandoc --reference-doc pandocTheme.docx -f html -t docx -o DailyTS.docx https://dli-it.gitlab.io/mkdocs/HRW-DevDocs/payroll-management/wagetype-based-timesheet/
---------------------------------

set "DOCSEARCH_ENABLED=true" && set "DOCSEARCH_ENGINE=lunr" && gulp bundle:pack

## Theme
gulp preview:build

antora-playbook-author-mode.yml DDOCSEARCH_ENABLED=true DOCSEARCH_ENGINE=lunr antora site.yml

set "DOCSEARCH_ENABLED=true" && set "DOCSEARCH_ENGINE=lunr" && antora --generator antora-site-generator-lunr antora-playbook.yml


set "DOCSEARCH_ENABLED=true" && set "DOCSEARCH_ENGINE=lunr" && antora --generator antora-site-generator-lunr author-mode.yml

http-server build/site -c-1 -p 5000 DDOCSEARCH_ENABLED=true DOCSEARCH_ENGINE=lunr antora site.yml


# Antora commands

``` python linenums="1"
antora antora-playbook.yml
antora --fetch antora-playbook.yml
antora --fetch author-mode.yml 
```

``` python linenums="1"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```

## Local site preview

set "DOCSEARCH_ENABLED=true" && set "DOCSEARCH_ENGINE=lunr" && antora --generator antora-site-generator-lunr local-playbook.yml

## Serve
1. Install
npm i -g http-server
yarn global add http-server

2. Serve
http-server build/site -c-1
http-server build/site -c-1 -p 5000
-c-1 flag to disable caching



pandoc -f html -t asciidoctor -o PRL_PayrollSheet00.adoc PRL_PayrollSheet00.html 

UI bundle
gulp preview


npm i -g @asciidoctor/core asciidoctor-pdf
npm run clean-install and then npm run build

Reveal Presentation: C:\Users\Documentation\Documents\GitHub\doc-dli.gitlab.io\node_modules\.bin\asciidoctor-revealjs.cmd presentation.adoc


[%autowidth]
|===
| A
| B
| C
|===

Mindfulness
https://www.youtube.com/watch?v=7-bPYMAdnnM
https://www.youtube.com/watch?v=h-CYAQqpvcw


---
Doctype book level 0 error

= Book Title
:chapter: 12
:sectnums: 
:sectnumoffset: 11  (chapter minus 1)
:leveloffset: 1

= Chapter Title


## Misc
 
gem install asciidoctor
 