---
layout: post
title:  "Markup your text with Markdown"
author: shiv
categories: [ tech ]
comments: false
image: assets/images/md.png
---
Not all content needs bell and whistles. Notepad style text is boring as well. Here is where we have a formatting standard called **Markdown** come to the rescue. Markdown is a simple text based formatting that anyone can do using a simple text editor and when it is processed by the right rendering engine, you get formatted text. It is much simpler than **html** and can very conveniently be used to write web based documents. You can learn markdown 101 [here](https://www.markdownguide.org/basic-syntax/) and [Wikipedia](https://en.wikipedia.org/wiki/Markdown) has all the details you would be interested in knowing about markdown, including its history. In this article I am sharing some of the more advanced things that you can do using markdown.


## Special formatting

As well as bold and italics, you can also use some other special formatting in Markdown when the need arises, for example:

+ ~~strike through~~
+ Large dashes using `---` which render as  --- inline
+ Adding color using html like `<font color="LimeGreen">This text is lime green!</font>` renders as <font color="LimeGreen">This text is Lime Green in color!</font>


## Writing code blocks

There are two types of code elements which can be inserted in Markdown, the first is inline, and the other is block. Inline code is formatted by wrapping any word or words in back-ticks, `like this could be some inline code`. Larger snippets of code can be displayed across multiple lines using triple back ticks followed by a name of the code language.

#### No language hint
```
.my-link {
    text-decoration: underline;
}
```

#### HTML

```html
<li class="ml-1 mr-1">
    <a target="_blank" href="#">
    <i> Here I come </i>
    </a>
</li>
```

#### CSS

```css
.highlight .c {
    color: #999988;
    font-style: italic; 
}
.highlight .err {
    color: #a61717;
    background-color: #e3d2d2; 
}
```

#### JS

```js
// alertbar later
$(document).scroll(function () {
    var y = $(this).scrollTop();
    if (y > 280) {
        $('.alertbar').fadeIn();
    } else {
        $('.alertbar').fadeOut();
    }
});
```

#### Python

```python
print("Hello World")
```

## Reference lists

Other than the standard `[Text](url)` markdown format, another way to insert links in markdown is using reference lists. You might want to use this style of linking to cite reference material like in a publication. All of the links are listed at the end of the document, so you can maintain full separation between content and its source or reference.

The links below have been rendered using Reference Style markdown shown in the code box below it.
> Here is [Wikipedia][1], the free encyclopedia and who knew that [Chemistry][2] dot com would be a dating site!

[1]: <https://en.wikipedia.org/> "Wikipedia"
[2]: <https://www.chemistry.com> "Meet other singles"

```
Here is [Wikipedia][1], the free encyclopedia and who knew that [Chemistry][2] dot com would be a dating site!

[1]: <https://en.wikipedia.org/> "Wikipedia"
[2]: <https://www.chemistry.com> "Meet other singles"
```


## Escape into HTML

We saw a nifty trick earlier to add color to your markdown text using `<font>` but the fact is that you can use full html within Markdown. Below is an embed code that has been iframed into markdown. This is no different from what you would otherwise write into an html document.

Below is an embedded video into markdown!

<p style="text-align:center"><iframe style="width:50%; height:300px" src="https://www.youtube.com/embed/P3RXtoYCW4M?rel=0&amp;showinfo=0" frameborder="0" allowfullscreen></iframe></p>