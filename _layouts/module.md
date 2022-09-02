---
layout: default
---
<h1>{{page.title}}</h1>
<span style="float: right; width: 200px; text-align: right;"><a id="spanish-link" href="#" style="display: none; border: none;">Español</a></span>

{{page.description}}

<p><hr/></p>

{{ content }}

<div id="codex-pathway" style="display: none;"><i>This module is part of the Level {{page.level}} WebDev Pathway at CodeX Academy. For more information, <a href="https://webdev.codex.academy/{{page.level}}">click here</a>.</i></div>

<p><hr/></p>

<p>Maintained by <a href='https://codex.academy'>CodeX Academy</a> and <a href='https://growstrong.io'>Grow Strong</a>.<br/>
Found a bug? <a href='{{site.github.repository_url}}/issues}}'>Report it</a> or <a href="{{site.github.repository_url}}/blob/master/{{page.path}}">Edit this page</a>. Want to contribute? <a href="{{ link /contributing.md }}">Pitch in!</a></p>

<script>
setTimeout(()=> {
    if({{page.hasSpanish}}){
        const url = "{{site.url}}{{page.url}}";
        const es_url = url.replace(".html","-es.html");
        const link = document.getElementById("spanish-link");
        link.href = es_url;
        link.style.display = "block";
    }
    if({{page.level}}){
        const section = document.getElementById("codex-pathway");        
        section.style.display = "block";
    }
}, 500);
</script>

<style>
#codex-pathway { padding: 20px; position: absolute; top: 20px; right: 20px; border-radius: 20px; background-color: #EEEEEE; }
</style>