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
> Here is an info blockquote without icon

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



