---
layout: default
---
<h1>Design Pattern: {{page.title}}</h1>
<span style="float: right; width: 200px; text-align: right;"><a id="spanish-link" href="#" style="display: none;">Español</a></span>

<p>A developer who can proficiently implement the "{{page.title}}" design pattern as well as recognize situations where it is appropriate.</p>

<p><hr/></p>

<h2>Master the following skills:</h2>

<ul>
    <li>Compare/contrast this design pattern to other design patterns</li>
    <li>Describe the design pattern to less experienced developers</li>
    <li>Recognize situations where this design pattern is appropriate</li>
    <li>Implement the design pattern correctly from memory</li>
    <li>Code the design pattern using TDD (unit tests first)</li>
</ul>

<h2>Suggested Learning:</h2>

<ul>
    <li><a href="https://refactoring.guru/design-patterns" target="_blank">Design Pattern Guru</a></ul>
    <li><a href="https://www.dofactory.com/" target="_blank">Do Factory</a></ul>
    <li><a href="https://www.coursera.org/learn/design-patterns" target="_blank">Design Patterns Courses</a> from Courera</ul>
    <li><a href="https://www.udemy.com/course/typescript-design-patterns/" target="_blank">TypeScript Design Patterns</a></ul>
    <li><a href="https://www.youtube.com/playlist?list=PLrhzvIcii6GNjpARdnO4ueTUAVR9eMBpc" target="_blank">Design Patterns in Object Oriented Programming</a></ul>
</ul>

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