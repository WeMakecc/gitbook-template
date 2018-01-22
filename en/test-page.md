# Heading H1

## Heading H2

### Heading H3

#### Heading H4

##### Heading H5

###### Heading H6

---

# This an H1 Heading with a "\#title" id {#title}

---

# Paragraphs {#paragraphs}

Regular paragraph text

**Bold text**

_Italic text_

_**Bold and italic text**_

~~Strikethrough text~~

---

# Lists {#lists}

1. First ordered list item
2. Another item
   * Unordered sub-list.
3. Actual numbers don't matter, just that it's a number
   1. Ordered sub-list
4. And another item.

   You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces \(at least one, but we'll use three here to also align the raw Markdown\).

   To have a line break without a paragraph, you will need to use two trailing spaces.  
   Note that this line is separate, but within the same paragraph.  
   \(This is contrary to the typical GFM line break behaviour, where trailing spaces are not required.\)

5. And another item after a lot of text


6. You can start a new list after two line breaks

---

# Tasks list {#tasks}

- [ ] task 1
- [x] task 2

---

# Links {#links}

You can link to a [heading within the same article](#title) or to [an heading in another article](/chapter-1/content.md#content)

You can link to an [article](/chapter-1/content.md)
(but if you are linking to a `readme` file you need to use a special syntax `[article](/chapter-1/README.md/#readme)`)

You can of course always link to [whatever web address](http://www.google.com)

---

# Footnotes {#footnotes}

footnote[^1]

footnote [link](/www.google.com)[^2]

[^1]: this is a plain footnote

[^2]: link: [http://www.google.com](http://www.google.com)

---

# Code {#code}

```
this is a
code block
```

```css
/* this is a code block with syntax highlighting */  
#title {  
  padding-bottom: .2rem;  
  border-bottom: 1px solid #eaecef;  
}
```

this is inline `code` instead

this is code included from the `timer.ino` file in the `code` folder:
[include](../code/timer.ino)

---

# Blockquote {#blockquote}

> this is a very famous quote, you should read it 'cause it will make you smarter.
>
> and it can continue on a second paragraph.  
> and you can also have a single line break without starting a new paragraph

---

# Special blockquotes {#specialblockquote}

> **info**
> This is an info blockquote with icon (the icon will not render in the PDF...)

(you need characters in between two sequential blockquotes)

> **info no-icon**
> This is an info blockquote without icon

(you need characters in between two sequential blockquotes)

> **tip**
> This is a tip blockquote with icon (the icon will not render in the PDF...)

(you need characters in between two sequential blockquotes)

> **tip no-icon**
> This is a tip blockquote without icon

(you need characters in between two sequential blockquotes)

> **danger**
> This is a danger blockquote with icon (the icon will not render in the PDF...)

(you need characters in between two sequential blockquotes)

> **danger no-icon**
> This is a danger blockquote without icon

(you need characters in between two sequential blockquotes)

> **success**
> This is a success blockquote with icon (the icon will not render in the PDF...)

(you need characters in between two sequential blockquotes)

> **success no-icon**
> This is a success blockquote without icon

---

# Tables

|you|can|create|tables|
|-|-|-|-|
|no matter the amount|of columns or rows|as long as you remember that tables are fluid and not responsive, and usually have layout problems with smaller resolutions||
|another row|it looks alternated|and can have one less column|
|some markdown syntax is accepted in cells|**bold text**|![](../assets/rodrigomuller-acdc.jpg)|_italic text_|
|<ol><li>of course</li><li>you can</li><li>have html</li><li>in a cell</li></ol>|

---

# Images {#images}

<img src="../assets/rodrigomuller-acdc.jpg" alt="caption text" width="50%" align="left" style="margin-right:10px">
You can have images aligned to the left with a tiny bit of HTML
```html

<img src="../assets/rodrigomuller-acdc.jpg" width="50%" align="left" style="margin-right:10px">

```
but in order to not break the flow, the text should wrap the image in its entirety, so you need to be sure the ratio between the image size and the amount of text is good. You can also decide the image size in the `image` tag with the `width` attribute. It can be expressed absolutely in px, or relatively in %. If you don't declare the `height` attribute the image will resize accordingly.

<img src="../assets/rodrigomuller-acdc.jpg" width="100px" align="right" style="margin-left:10px">
Of course images can also be aligned to the right, just be sure the ration between the image size and the amount of text will always make the text wrap the image. This can be tricky at times, so to reach a good output layout you might do some trial and error.

Also, please remember that if you are supporting PDF output, the resolution for the PDF is different so do some export tests to check it's not breaking the PDF layout.

###### A list of images with description on the right
<p style="overflow:hidden"><img src="../assets/rodrigomuller-acdc.jpg" width="150px" align="left" style="margin-right:10px">
You can achieve such a result with a little bit of HTML, but unfortunately you won't be able to use markdown syntax anymore :(
</p>  


<p style="overflow:hidden"><img src="../assets/rodrigomuller-acdc.jpg" width="150px" align="left" style="margin-right:10px">
When trying some _markdown_ syntax it **will** just be rendered as regular HTML text...
</p>

Please check the code snippet below to see the HTML used to render the layout above:
```html
<p style="overflow:hidden"><img src="../assets/rodrigomuller-acdc.jpg" width="150px" align="left" style="margin-right:10px">
You can achieve such a result with a little bit of HTML, but unfortunately you won't be able to use markdown syntax anymore :(
</p>  


<p style="overflow:hidden"><img src="../assets/rodrigomuller-acdc.jpg" width="150px" align="left" style="margin-right:10px">
When trying some _markdown_ syntax it **will** just be rendered as regular HTML text...
</p>
```

<img src="../assets/rodrigomuller-acdc.jpg" align="center" alt="center aligned images can have a caption">

---

# Video {#video}

You can embed videos in a gitbook. They will be displayed as an interactive element in website view and as a link in PDF view.

Videos can be embedded from youtube:
{{ 'https://www.youtube.com/watch?v=U0sZulbldWg' | video }}

From Vimeo:
{{ 'https://vimeo.com/174632471' | video }}


---

# PDF embed {#pdf}

It is also possible to embed PDF files in the gitbook.
[Please note that, unfortunately, the generated links are broken in the PDF downloaded from gitbook.com]

{% pdf src="../assets/opencare-graphic-guide.pdf", width="100%", height="700" %}{% endpdf %}

---

# Book Cover {#cover}

It is possible to add a cover for the PDF and Ebook versions of the book.
There are two possible ways of adding a cover.

**Auto cover plugin**
Open the `book.json` file in the root directory of your book and:
* edit the `"title": "My Book"` value with your book title
* edit the `"author": "Author"` value with your book author details
* scroll down, find the `pluginsConfig` and `autocover` keys and
  * inside the `font` value you can:
    * edit the `size` value with desired font size (20 min suggested)
    * edit the `family` value with the desired font face (for a list of web safe fonts please check [here](https://www.w3schools.com/cssref/css_websafe_fonts.asp)) 
    * edit the `color` value with your desired hex color (this would only affect the font color)
  * leave the `size` value unchanged
  * inside the `background` value you can edit the `color` value with your desired background color in hex


**Custom cover**
Create an artwork with the software of your choice following this criteria:
* Save the file in `JPEG` format with name `cover.jpg` in the root of the directory of the book. Adding a `cover_small.jpg` will specify a smaller version of the cover.
* Size of 1800x2360 pixels for `cover.jpg`, 200x262 for `cover_small.jpg`

When you are done please head to the `book.json` file in the root directory of your book and:
* delete the `"autocover"` value inside the `"plugins"` array
* delete the
```
"autocover": {
            "font": {
                "size": null,
                "family": "Impact",
                "color": "#FFF"
            },
            "size": {
                "w": 1800,
                "h": 2360
            },
            "background": {
                "color": "#09F"
            }
        }
```
found inside the `pluginsConfig` key

**_IMPORTANT_** Please, when deleting code from the `book.json`, always make sure you also remove the comma that might precede the line you want to remove. _The build of the book will break otherwise_

For instance, remove the last comma in this situation
```
"plugins": [
        "anchorjs",
        "styled-blockquotes",
        "todo",
        "include-codeblock",
        "ace",
        "copy-code-button",
        "image-captions",
        "noembed",
        "embed-pdf",
    ]
```
Correct syntax:
```
"plugins": [
        "anchorjs",
        "styled-blockquotes",
        "todo",
        "include-codeblock",
        "ace",
        "copy-code-button",
        "image-captions",
        "noembed",
        "embed-pdf"
    ]
```

---

{% image "test image", "200px", "left", "margin-right:10px" %}
    {% image_url %}../assets/rodrigomuller-acdc.jpg
    {% image_text %}lalalalala lalalala lalalala
{% endimage %}


---


{% grid %}
  {% col 1 %}First
  {% col 2 %}Second
  {% col 3 %}Third
{% endgrid %}