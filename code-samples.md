---
title: Markdown Samples
has_children: true
nav_order: 3
has_toc: false
---

# Markdown samples

## Text

    It's very easy to make some words **bold** and other words *italic* with Markdown. 
    You can even [link to Google!](http://google.com)
    
It's very easy to make some words **bold** and other words *italic* with Markdown. 
You can even [link to Google!](http://google.com)

## Headers
    # This is an <h1> tag
    ## This is an <h2> tag
    ###### This is an <h6> tag
    
## Emphasis
    *This text will be italic*
    _This will also be italic_

    **This text will be bold**
    __This will also be bold__

    _You **can** combine them_
    
For example:

*This text will be italic*

_This will also be italic_

**This text will be bold**

__This will also be bold__

_You **can** combine them_

There's a horizontal rule below this.

* * *

the code is:

    * * *
    

## Lists

### Unordered

    * Item 1
    * Item 2
      * Item 2a
      * Item 2b

### Ordered
  
    1. Item 1
    1. Item 2
    1. Item 3
       1. Item 3a
       1. Item 3b

## Nested Lists
You can create a nested list by indenting one or more list items below another item.

    1. First list item
       - First nested list item
         - Second nested list item
         
    - first item
    - second item
      - indent 1
      - indent 2
    - third item
    
Would be:
 1. First list item
       - First nested list item
         - Second nested list item
         
- first item
- second item
  - indent 1
  - indent 2
- third item

### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

## Images

    ![GitHub Logo](/images/logo.png)
    Format: ![Alt Text](url)

## Links

You can create an inline link by wrapping link text in brackets [ ], and then wrapping the URL in parentheses ( ). You can also use the keyboard shortcut command + k to create a link.

    http://github.com - automatic!
    [GitHub](http://github.com)

## Relative links

You can define relative links and image paths in your rendered files to help readers navigate to other files in your repository.

A relative link is a link that is relative to the current file. For example, if you have a README file in root of your repository, and you have another file in docs/CONTRIBUTING.md, the relative link to CONTRIBUTING.md in your README might look like this:

    [Contribution guidelines for this project](docs/CONTRIBUTING.md)

GitHub will automatically transform your relative link or image path based on whatever branch you're currently on, so that the link or path always works. You can use all relative link operands, such as ./ and ../.

Relative links are easier for users who clone your repository. Absolute links may not work in clones of your repository - we recommend using relative links to refer to other files within your repository.

## Blockquotes

    As Kanye West said:

    > We're living the future so
    >
    > the present is our past.
    
Would look like this:

As Kanye West said:

> We're living the future so
>
> the present is our past.

## Inline code

    I think you should use an
    `<addr>` element here instead.
    
 Would look like this:
 
 I think you should use an `<addr>` element here instead.
 
 ```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```
 
## GitHub Flavoured Markdown

GitHub.com uses its own version of the Markdown syntax that provides an additional set of useful features, many of which make it easier to work with content on GitHub.com.

Note that some features of GitHub Flavored Markdown are only available in the descriptions and comments of Issues and Pull Requests. These include @mentions as well as references to SHA-1 hashes, Issues, and Pull Requests. Task Lists are also available in Gist comments and in Gist Markdown files.

## Syntax highlighting
Here’s an example of how you can use syntax highlighting with GitHub Flavored Markdown:

```javascript
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }
}
```
You can also simply indent your code by four spaces:

    function fancyAlert(arg) {
      if(arg) {
        $.facebox({div:'#foo'})
      }
    }

Here’s an example of Python code without syntax highlighting:

    def foo():
        if not bar:
            return True

This is another example:

    Some basic Git commands are:
```
git status
git add
git commit
```
would look like:

Some basic Git commands are:
```
git status
git add
git commit
```

## Task Lists

    - [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
    - [x] list syntax required (any unordered or ordered list supported)
    - [x] this is a complete item
    - [ ] this is an incomplete item

this code displays as:

- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item

If you include a task list in the first comment of an Issue, you will get a handy progress indicator in your issue list. It also works in Pull Requests!

If a task list item description begins with a parenthesis, you'll need to escape it with \:

    - [ ] \(Optional) Open a followup issue

## Tables

You can create tables by assembling a list of words and dividing them with hyphens - (for the first row), and then separating each column with a pipe `|`:

    First Header | Second Header
    ------------ | -------------
    Content from cell 1 | Content from cell 2
    Content in the first column | Content in the second column

Would become:

First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column

this is another table style:

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

the code is:

    | head1        | head two          | three |
    |:-------------|:------------------|:------|
    | ok           | good swedish fish | nice  |
    | out of stock | good and plenty   | nice  |
    | ok           | good `oreos`      | hmm   |
    | ok           | good `zoute` drop | yumm  |

## Automatic linking for URLs

Any URL (like `http://www.github.com/`) will be automatically converted into a clickable link.

## Strikethrough

Any word wrapped with two tildes (like `~~this~~`) will appear crossed out.

For example:

~~text~~

## Emojis

Once the jemoji plugin has been added to the config.yml file, any emojis can be added to the page.

I give this plugin two :+1:!

The light bulb could be handy for notes - :bulb:
