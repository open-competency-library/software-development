---
layout: default
---
<h1>Design Pattern: {{page.title}}</h1>
<span style="float: right; width: 200px; text-align: right;"><a id="spanish-link" href="#" style="display: none;">Español</a></span>

A developer who can proficiently implement the "{{page.title}}" design pattern as well as recognize situations where it is appropriate.

<p><hr/></p>

## Master the following skills:

- Compare/contrast this design pattern to other design patterns
- Describe the design pattern to less experienced developers
- Recognize situations where this design pattern is appropriate
- Implement the design pattern correctly from memory
- Code the design pattern using TDD (unit tests first)

## Suggested Learning:

- [Design Pattern Guru](https://refactoring.guru/design-patterns){:target="\_blank"}
- [Do Factory](https://www.dofactory.com/){:target="\_blank"}
- [Design Patterns Course](https://www.coursera.org/learn/design-patterns){:target="\_blank"} from Coursera
- [TypeScript Design Patterns](https://www.udemy.com/course/typescript-design-patterns/){:target="\_blank"}
- [Design Patterns in Object Oriented Programming](https://www.youtube.com/playlist?list=PLrhzvIcii6GNjpARdnO4ueTUAVR9eMBpc){:target="\_blank"}

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