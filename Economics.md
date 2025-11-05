---
layout: page
title: Economics
permalink: economics

patents:
-   number: 10143052
    string: "10,143,052"
    name: Light Emitting Diode (LED) Warm on Dim Circuit


---
<div class="grid grid-cols-8 font-sans pl-32 pt-4 pb-16 prose-{{site.theme-color}} font-mono">
    {% for patent in page.patents %}
        <div class="col-span-1 text-right pr-4">
            {{patent.string}}:
        </div>
        <div class="col-span-7">
            <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/{{patent.number}}" 
            target="_blank" rel="noopener noreferrer" class="underline text-blue-600"> 
                "{{patent.name}}"
            </a>
        </div>
    {% endfor %}
</div>
