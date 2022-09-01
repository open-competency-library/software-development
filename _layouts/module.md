---
layout: default
---
<span style="float: right; width: 200px; text-align: right;"><a id="spanish-link" href="#" style="display: hidden;">Español</a></span>
<h1>{{page.title}}</h1>

{{page.description}}

<p><hr/></p>

{{ content }}

<p><hr/></p>

<p>Maintained by <a href='https://codex.academy'>CodeX Academy</a> and <a href='https://growstrong.io'>Grow Strong</a>.<br/>
Found a bug? <a href='{{site.github.repository_url}}/issues}}'>Report it</a> or <a href="{{site.github.repository_url}}/blob/master/{{page.path}}">Edit this page</a>. Want to contribute? <a href="{{ link /contributing.md }}">Pitch in!</a></p>

<script>
setTimeout(()=> {
    const url = "{{site.url}}{{page.url}}";
    const es_url = url.replace(".html","-es.html");
    const link = document.getElementById("spanish-link");
    console.log("es_url", es_url);
    console.log("link", link);
    link.href = es_url;
    link.style.display = "inline";
}, 500);
</script>