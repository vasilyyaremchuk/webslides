+++
title = "Hugo-Webslides"
+++
<!--: bg-black .wrap .size-100 ..aligncenter ..background ..dark bgimage=images/pencil.jpg -->


## **Hugo-Webslides**
<!--: .text-intro -->Use markdown to write contents and render with [**WebSlides**](https://webslides.tv) to HTML.

[{{< svg fa-github >}}Github](https://github.com/RCJacH/hugo-webslides)

---
<!-- : .wrap -->

|||v

### **All from one markdown file**

Use three dashes "<code>-</code>" to create a separate slide page.

|||

~~~md

Slide1

---

Slide2

~~~

---
<!-- : .wrap -->


|||

~~~
content
├── home
│   ├── home1.md (weight: 1)
│   └── home2.md (weight: 2)
└── _index.md (initial page)
~~~

|||

### Or not.

You can combine and arrange files with the weight parameter in front matter, and categorize .md files into different folders.

---
<!-- : .wrap -->

### You can assign class to many elements

<!-- : .flexblock -->
- {{< flexblock "Slides" 6 >}}
<span><!-</span>- : sectionClass .divClass ..subClass -<span>-></span><br>
Content
~~~html
<section class="sectionClass">
  <div class="divClass">
    <div class="subClass">
    Content
    </div>
  </div>
</section>
~~~
{{< /flexblock >}}

- {{< flexblock "Headers and Paragraphs" 6 >}}
<span># <!-</span>- : .hClass -<span>-></span>Header<br>
<span><!-</span>- : .pClass -<span>-></span>Paragraph
~~~html
<h1 class="hClass">Header</h1>
<p class="pClass">Paragraph</p>
~~~
{{< /flexblock >}}

- {{< flexblock "Lists" 6 >}}
<span><!-</span>- : .listClass -<span>-></span><br>
<span>-</span> list1<br>
<span>-</span> list2
~~~
<ul class="listClass">
  <li>list1</li>
  <li>list2</li>
</ul>
~~~
{{< /flexblock >}}
