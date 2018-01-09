# Heading H1

## Heading H2

### Heading H3

#### Heading H4

##### Heading H5

###### Heading H6

---

# This an H1 Heading with a "\#title" id {#title}

---

Regular paragraph text

**Bold text**

_Italic text_

_**Bold and italic text**_

~~Strikethrough text~~

---

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

- [ ] task 1
- [x] task 2

---

footnote[^1]

footnote [link](/www.google.com)[^2]

[^1]: this is a plain footnote

[^2]: link: [http://www.google.com](http://www.google.com)

---

> this is a very famous quote, you should read it 'cause it will make you smarter.
>
> and it can continue on a second paragraph.  
> and you can also have a single line break without starting a new paragraph

---

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

info blockquote
> **[info] For info**
>
> Use this for infomation messages.


warning blockquote
> **[warning] For warning**
>
> Use this for warning messages.


danger blockquote
> **[danger] For danger**
>
> Use this for danger messages.


success blockquote
> **[success] For info**
>
> Use this for success messages.

---

This is some text that I would like to sit on the left of the image. The image is aligned to the right and width has been set to 50% <img src="../assets/rodrigomuller-acdc.jpg" width="50%" align="left">


This is some text that I would like to sit on the right of the image. The image is aligned to the left and width has been set to 50% <img src="../assets/rodrigomuller-acdc.jpg" width="50%" align="left">


<img src="../assets/rodrigomuller-acdc.jpg" align="center" alt="this image is center aligned, real width, and has a caption">








