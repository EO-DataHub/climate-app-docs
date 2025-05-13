---
title: Guidance for authors
icon: material/book-open-variant-outline
---
# Guidance for documentation authors

This page is a documentation page of guidance for writing docs with _MkDocs_ and _Material for MkDocs_ which includes basic information and guidance to help site authors.

## Deployment

* The site is currently deployed to [https://sparkgeo.github.io/climate-app-docs/] but this may change.
* The source is the docs section of our [uk_eodatahub] repo on GitHub.
* This page specifically is [here](https://github.com/sparkgeo/climate-app-docs/edit/main/docs/reference/documentation/x1-appendix-a.md)
  
  [https://sparkgeo.github.io/climate-app-docs/]: https://sparkgeo.github.io/climate-app-docs/
  [uk_eodatahub]: https://github.com/sparkgeo/climate-app-docs/edit/main/docs/
  
It takes a couple of minutes for updates to be deployed.  You can check the status of the update in the [actions](https://github.com/sparkgeo/climate-app-docs/actions) page in the repo.

## Markdown primer

### Guidance

This [markdown guide] is a pretty **comprehensive overview** that covers the main points of markdown.  The [Material for MKDocs] reference should also be consulted for more advanced features.

[markdown guide]: https://www.markdownguide.org/basic-syntax/#overview
[Material for MKDocs]: https://squidfunk.github.io/mkdocs-material/

The basic markdown can be previewed directly in GitHub and should then render well to Material for MKDocs.

Some examples are:

### Fonts and headings

Basics include _italics_, **bold** and headings such as

### Level 3 heading

#### Level 4 heading

##### Level 5 heading

etc

### Tables

| A | B |
|---|---|
|123|456|

See also the extended syntax in the [markdown guide] for things like table alignment

### Block sections

> Block text
> is done with > signs like this.
>
> It **can also include formatting** such as **bold**, _italics_, _**both**_ and
>
> * lists
> * like this one
>
> #### Headings like this one
>
> And so on

### Code words

If you had say a `filename` that you wanted to reference, then using the backtick markdown, which is top left on your keyboard beneath the `escape` key is a where you'll find it.

### Code blocks

We proably will not need this for our but here are a few examples.

    Indenting text by 4 spaces (2 tabs) adds it like this, with courier font
    grey background and line breaks
    as
    they
    are written.
    It probably also escapes any characters that might otherwise be thought of as markdown.

Syntax highlighting to a specific language is done like this.

```python
def greet(name):
    return f"Hello, {name}!"

print(greet("World"))
```

    ```python
    def greet(name):
        return f"Hello, {name}!"
    
    print(greet("World"))
    ```
    

### Admonitions

An admonition is essentially like a block section or callout with additional formatting.  I don't think this is core markdown but is instead supported variably by the rendering tools such as MkDocs that are used to display it, with details on the [admonitions] page at MkDocs.  Note, this does require a bit some updates to the mkdocs.yml file as described in those docs.   Anyway some good examples are

!!! note
    The note itself is specified by _!!! note_ on the first line, and then this content is indented. This will also add in the icon, colour etc.

!!! warning
    The alighment of the text in the block is important though, and you need to tab it out twice (or with 4 spaces) until it diplays underneath the word note.

!!! note "Note with a custom title
    First line is _!!! note "Title words"_ then content is indented
  
!!! note ""
    When first line is _!!! note ""_ there is no title.

!!! tip
    There are a whole load of other Admonitions not just note, such as:
    *tip
    * abstract
    *info
    * success
    *warning
    * failure
    *bug
    * example
    * quote
    If you want the details, check out the [admonitions] page at **MkDocs**

[admonitions]: https://squidfunk.github.io/mkdocs-material/reference/admonitions/

!!! info inline "Inline admonitions"
    Adding the "inline" modifier after !!! also allows you to create an an admoniition like this which other text wraps around.

**NOTE** Admonitions using "inline" need to be included before the conent that you want wrapping around it (i.e. this block of text).  If you want the inline to be to the right hand side of the block of text then you also need to add in an "end" modifier, but presumably with the same sturcture (i.e. content being added afterwards as well).

!!! info inline end "Right aligned admonitions"
    Adding the "end" modifier "inline" after !!! also allows you to create a right aligned admonition.

I hoped a line break (two spaces at end of line and carriage return) which I've done here can avoid next text being wrapped.  

_But_ this is the next text after the break and it isn't so not sure how that can be controlled.

### Footnotes

It is also possible to add a footnote like this [^1] or this [^2] which appear at the bottom.  Note, "-footnotes" has been added to the mkdocs.yml file to make these work.

[^1]: And where I am a short footnote on a single line
[^2]:
    And I am a paragraph of footnotes that may
    actually span a number of lines if there is lots of content
    in the footnote.  This needs to be indented by four spaces
    which I think is the same as two tabs.

It took me a while to find the ^ character, but its `Shift-6`

### Horizontal rules

For a horizontal rule, three use three or more asterisks (***), dashes (---), or underscores (___) on a line by themselves.  Anyway lets drraw a line under this discussion for now (pun intended).
***

### Icons

MKDocs are deployed with Material icons, [https://pictogrammers.com/library/mdi/] is a good place to find them.
  [https://pictogrammers.com/library/mdi/]: <https://pictogrammers.com/library/mdi/>

### Hyperlinks

There are a number of options for doing hyperlinks in a page.

#### Simple inline link

Just wrapping a URL in "<" and ">" will display the address as a hyperlink.  This (and other examples here are documented at <https://www.markdownguide.org/basic-syntax/#links>.

#### Text hyperlinks

If you want the text to be different, for example [click here to jump out to Google](http://www.google.com), just pop the text in square brackets and the URL in round brackets straight after it.

#### Reference hyperlinks

Another type of link is a [reference hyperlink][RH].  So a [reference hyperlink][RH] is really useful when you want to use a [specific URL][RH] multiple times.  So [all the links][RH] in this paragraph all point to the same URL on the [markdown guide about reference hyperinks][RH] and as you can see we are using different text to point to the [same destiniation][RH] again and again.  In the body of text the we embed the text for the link in square bracktes, followed by another paid of square brackets for the reference and finally we define the URL for that reference later in the doc (with the reference in square brakets, a colon, then the URL.  This explanation is articulated better, in all the links in this paragraph.

[RH]: https://www.markdownguide.org/basic-syntax/#reference-style-links

#### Links to other pages in this doc repository

Links to other docs pages are probably all relative.

So this is the [owls page](/climate-app-docs/owls/) [this](/uk_eodatahub) would be the index page, and the [beetles page](/climate-app-docs/insects/beetles) although these pages are no longer in the repo!

    So this is the [owls page](/climate-app-docs/owls/)  
    [this](/uk_eodatahub) would be the index page, and the 
    [beetles page](/climate-app-docs/insects/beetles).

This [Appendix page][AP] is done as a reference link.
[AP]: /climate-app-docs/xxx-questions.md

### Images

Here is an image.

![Hazard indicator alt text](/climate-app-docs/user%20guide/images/hazards/1.png "Hazard indicator title")

Defined like this:
    ![Hazard indicator alt text](/climate-app-docs/user%20guide/images/hazards/1.png "Hazard indicator title")

### Where can I find out more about Material MK Docs?

Look at [https://squidfunk.github.io/mkdocs-material/reference/]
  [https://squidfunk.github.io/mkdocs-material/reference/]: <https://squidfunk.github.io/mkdocs-material/reference/>

### Ordering pages

* It seems to be _alphabetical_ by the name of the file in the repo.  The title of the file can be entirely different to its name, and the title is what is rendered.  So I've now prefixed this filename with _**xxx**_ so that it appears at the end of the index list.  So a file named _**aaa-introduction**_ with a _title_ of _Introduction_ would be first in the list.
* [This page] on the Material MkDocs site is not in alphabetical so there may also be another way of doing it
  