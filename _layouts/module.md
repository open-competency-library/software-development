---
layout: default
---
<h1>{{page.title}}</h1>
<span style="float: right; width: 200px; text-align: right;"><a id="spanish-link" href="#" style="display: none;">Español</a></span>

{{page.description}}

<p><hr/></p>

{{ content }}

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
#codex-pathway { 
    padding: 20px; 
    font-size: .8em; 
    border-radius: 20px; 
    background-color: #7253ed; 
    color: #ddd;
    text-align: center;
    margin-top: 20px;
    margin-bottom: 20px;
}
#codex-pathway a { color: white}
#spanish-link { background-image: none; }
</style>