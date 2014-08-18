Introductory RMarkdown
========================================================
author: Xiaojun Sun
date: July 23th, 2014
transition: rotate
font-family: 'Helvetica'


What's R?
========================================================
id: slide1

R is a language and environment for statistical computing and graphics. 

[R Homepage](http://www.r-project.org/)

[R Language Features](http://www.revolutionanalytics.com/r-language-features)

[90 second video for an introduction to R](https://www.youtube.com/watch?v=TR2bHSJ_eck)



What's Markdown?
========================================================
incremental: true

- Markdown, who R you?
- Markdown is a text-to-HTML conversion tool for web writers. Markdown allows you to write using an easy-to-read, easy-to-write plain text format, then convert it to structurally valid XHTML (or HTML).
- Thus, Markdown is two things: 

1. a plain text formatting syntax;
2. a software tool, written in Perl, that converts the plain text formatting to HTML.


What's Markdown?(cont'd)
========================================================
incremental: true

- Markdown's syntax is intended for one purpose: to be used as a format for writing for the web.
- Markdown is not a replacement for HTML, or even close to it. Its syntax is very small.
- For any markup that is not covered by Markdown's syntax, you simply use HTML itself. 


What's Markdown?(cont'd)
========================================================

For example, to add an HTML table to a Markdown article:

    This is a regular paragraph.

    <table>
        <tr>
            <td>Foo</td>
        </tr>
    </table>

    This is another regular paragraph.



Markdown: Syntax
========================================================
id: markdown

[Markdown Syntax (English Version)](http://daringfireball.net/projects/markdown/syntax)

[Markdown Syntax (Chinese Version)](http://wowubuntu.com/markdown/)

Block Elements
- [Paragraphs and Line Breaks](#/p)
- [Headers](#/header)
- [Blockquotes](#/blockquote)
- [Lists](#/list)
- [Code Blocks](#/precode)
- [Horizontal Rules]((#/hr))

Markdown: Syntax (cont'd)
========================================================

Span Elements
- [Links](#/link)
- [Emphasis](#/em)
- [Code](#/code)
- [Images](#/img)

Miscellaneous
- [Backslash Escapes](#/backslash)
- [Automatic Links](#/autolink)


Markdown: Paragraphs and Line Breaks
========================================================
type: subsection
incremental: true
id: p
A paragraph is simply one or more consecutive lines of text, separated by one or more blank lines. Markdown supports "hard-wrapped" text paragraphs.

When you want to insert a `<br />` break tag using Markdown, you end a line with two or more spaces, then type return.

Markdown: Headers
========================================================
type: subsection
incremental: true
id: header

Setext-style headers are "underlined" using equal signs and dashes. For example:

    This is an H1
    =============
    This is an H2
    -------------

Atx-style headers use 1-6 hash characters at the start of the line, corresponding to header levels 1-6. For example:

    # This is an H1
    ## This is an H2
    ###### This is an H6

Markdown: Blockquotes
========================================================
type: subsection
id: blockquote

Markdown uses email-style `>` characters for blockquoting. 

    > This is the first level of quoting.
    >
    > > This is nested blockquote.
    >
    > Back to the first level.

It looks like
> This is the first level of quoting.
>
> > This is nested blockquote.
>
> Back to the first level.

Markdown: Lists
========================================================
type: subsection
id: list
Markdown supports ordered (numbered) and unordered (bulleted) lists. Unordered lists use `*`, `+`, and `-` followed by at least one space -- interchangably -- as list markers. Such as

    - Red
    - Green
    - Blue
It looks like
- Red
- Green
- Blue

Markdown: Lists (cont'd)
========================================================
type: subsection
Ordered lists use numbers followed by periods:

    1. Bird
    3. McHale
    2. Parish
It looks like

1. Bird
3. McHale
2. Parish

The number doesn't matter.


Markdown: Code Blocks
========================================================
type: subsection
id: precode

To produce a code block in Markdown, simply indent every line of the block by at least 4 spaces or 1 tab. For example:

    Here is an example of AppleScript:

        tell application "Foo"
            beep
        end tell
        

One level of indentation -- 4 spaces or 1 tab -- is removed. 

Here is an example of AppleScript:

    tell application "Foo"
        beep
    end tell

Markdown: Horizontal Rules
========================================================
type: subsection
id: hr

You can produce a horizontal rule tag (`<hr />`) by placing three or more hyphens, asterisks, or underscores on a line by themselves. If you wish, you may use spaces between the hyphens or asterisks. Each of the following lines will produce a horizontal rule:

    * * *

    ***

    *****

    - - -

    ---------------------------------------


Markdown: Links
========================================================
type: subsection
id: link

Markdown supports two style of links: *inline* and *reference*.
To create an inline link, use a set of regular parentheses immediately after the link text's closing square bracket.  For example:

    This is [an example](http://example.com/ "Title") inline link.

    [This link](http://example.net/) has no title attribute.
And

    [WISE](http://www.wise.xmu.edu.cn/index.asp)
    
will create link to 
[WISE](http://www.wise.xmu.edu.cn/index.asp)

Markdown: Links (cont'd)
========================================================
type: subsection

Reference-style links use a second set of square brackets, inside
which you place a label of your choosing to identify the link:

    This is [an example][id] reference-style link.
    
Then, anywhere in the document, you define your link label like this, on a line by itself:

    [id]: http://example.com/  "Optional Title Here"

Markdown: Links (cont'd)
========================================================
type: subsection

Here's an example of reference links in action:

    I get 10 times more traffic from [Google] [1] than from
    [Yahoo] [2] or [MSN] [3].

    [1]: http://google.com/        "Google"
    [2]: http://search.yahoo.com/  "Yahoo Search"
    [3]: http://search.msn.com/    "MSN Search"

Markdown: Links (cont'd)
========================================================
type: subsection

Using the implicit link name shortcut, you could instead write:

    I get 10 times more traffic from [Google][] than from
    [Yahoo][] or [MSN][].

    [google]: http://google.com/        "Google"
    [yahoo]:  http://search.yahoo.com/  "Yahoo Search"
    [msn]:    http://search.msn.com/    "MSN Search"
Both give you:

I get 10 times more traffic from [Google][] than from [Yahoo][] or [MSN][].

[google]: http://google.com/        "Google"
[yahoo]:  http://search.yahoo.com/  "Yahoo Search"
[msn]:    http://search.msn.com/    "MSN Search"

Markdown: Emphasis
========================================================
type: subsection
id: em
Markdown treats asterisks (`*`) and underscores (`_`) as indicators of emphasis. 
E.g., this input:

    *single asterisks*
    
    _single underscores_
    
    **double asterisks**
    
    __double underscores__


Markdown: Emphasis (cont'd)
========================================================
type: subsection

They will produce:

*single asterisks*

_single underscores_

**double asterisks**

__double underscores__


Markdown: Code
========================================================
type: subsection
incremental: true
id: code

To indicate a span of code, wrap it with backtick quotes (`` ` ``). Unlike a pre-formatted code block, a code span indicates code within a
normal paragraph. For example:

    Use the `read.table()` function.

will produce:

Use the `read.table()` function.

To include a literal backtick character within a code span,

    ``There is a literal backtick (`) here.``
    
``There is a literal backtick (`) here.``


Markdown: Images
========================================================
type: subsection
incremental: true
id: img

Markdown uses an image syntax that is intended to resemble the syntax for links, allowing for two styles: *inline* and *reference*.

Inline image syntax looks like this:

    ![Alt text](/path/to/img.jpg)

    ![Alt text](/path/to/img.jpg "Optional title")


Markdown: Images (cont'd)
========================================================
type: subsection

Reference-style image syntax looks like this:

    ![Alt text][id]

Where "id" is the name of a defined image reference. Image references are defined using syntax identical to link references:

    [id]: url/to/image  "Optional title attribute"


Markdown: Images (cont'd)
========================================================
type: subsection
For example,

    ![XMU, Lotus Lake](http://i.imgbox.com/NN29CSyH.jpg "XMU, Lotus Lake")
It will insert photo here:

![XMU, Lotus Lake](http://i.imgbox.com/NN29CSyH.jpg "XMU, Lotus Lake")


Markdown: Automatic Links
========================================================
type: subsection
id: autolink

Markdown supports a shortcut style for creating "automatic" links for URLs and email addresses: simply surround the URL or email address with angle brackets. 

You can do this:

    <http://www.xmu.edu.cn/>
Markdown will turn this:
http://www.xmu.edu.cn/


Markdown: Backslash Escapes
========================================================
type: subsection
id: backslash

Markdown allows you to use backslash escapes to generate literal characters which would otherwise have special meaning in Markdown's formatting syntax.

If you wanted to surround a word with literal asterisks, you can use backslashes before the asterisks, like this:

    \*literal asterisks\*
It gives you: 

\*literal asterisks\*


RMarkdown: Introduction
========================================================
incremental: true

> R Markdown is an authoring format that enables easy creation of dynamic documents, presentations, and reports from R. It combines the core syntax of markdown with embedded R code chunks that are run so their output can be included in the final document. R Markdown documents are fully reproducible (they can be automatically regenerated whenever underlying R code or data changes).

This is what I want to show you! 


RMarkdown: Syntax
========================================================
- [Markdown Basics](#/markdown)
- [R Code Chunks](#/rcodeCh)
- [Inline R Code](#/inlineR)
- [Embedding Equations](#/equa)
- [Output Options](#/out)
- [Shiny](#/shiny)
- [knitr package](#/knirtpack)




RMarkdown: R Code Chunks
========================================================
type: subsection
id: rcodeCh


```r
summary(cars)
```

```
     speed           dist    
 Min.   : 4.0   Min.   :  2  
 1st Qu.:12.0   1st Qu.: 26  
 Median :15.0   Median : 36  
 Mean   :15.4   Mean   : 43  
 3rd Qu.:19.0   3rd Qu.: 56  
 Max.   :25.0   Max.   :120  
```


RMarkdown: R Code Chunks (cont'd)
========================================================
type: subsection

```r
library(ggplot2)
qplot(speed, dist, data=cars)+geom_smooth()
```

![plot of chunk unnamed-chunk-2](introductory_rmarkdown-figure/unnamed-chunk-2.png) 



RMarkdown: Inline R Code
========================================================
type: subsection
id: inlineR

You can also evaluate R expressions inline by enclosing the expression within a single back-tick qualified with `r`. For example, 


```r
x=2
y=45
```

Then the following code:

    I get ` r x` jobs and each pays me ` r y` a day. Then I earn $ ` r x*y` a day.

(remove the space before `r`) gives you:

I get 2 jobs and each pays me $ 45 a day. Then I earn $ 90 a day.


RMarkdown: Embedding Equations
========================================================
type: subsection
id: equa

You can embed LaTeX or MathML equations in R Markdown files using the following syntax:
- `$equation$` for inline equations (note there must not be white space adjacent to the $ delimiters)
- `$$ equation $$` for display equations
- `<math ...> </math>` for MathML equations.


RMarkdown: Embedding Equations (cont'd)
========================================================
type: subsection

    The combined forecast is:
    $$Y_{t,1}^{c}=kY_{t,1}^{1}+(1-k)Y_{t,1}^{2}$$
It gives you: 

The combined forecast is: 
$$Y_{t,1}^{c}=kY_{t,1}^{1}+(1-k)Y_{t,1}^{2}$$

    The Arithmetic mean is equal to $\frac{1}{n} \sum_{i=1}^{n} x_{i}$.

will give you:

The Arithmetic mean is equal to $\frac{1}{n} \sum_{i=1}^{n} x_{i}$.



RMarkdown: Output Options
========================================================
type: subsection
id: out

R Markdown documents can contain a metadata section that includes both title, author, and date information as well as options for customizing output. 

    ---
    title: "Sample Document"
    output:
      html_document:
        toc: true
        theme: united
      pdf_document:
        toc: true
        highlight: zenburn
    ---

RMarkdown: Shiny
========================================================
type: subsection
id: shiny
    shiny::runGitHub("shiny-js-examples", "jcheng5", subdir="output")
![Shiny interactive plot](http://rmarkdown.rstudio.com/images/shiny-interactive-plot.png)



RMarkdown: knitr package
========================================================
type: subsection
id: knirtpack
Elegant, flexible and fast dynamic report generation with R

The knitr package was designed to be a transparent engine for dynamic report generation with R.

[knitr package options](http://yihui.name/knitr/options)

You needn't know all of them.


RMarkdown: Editor
========================================================
[StackEdit ](https://stackedit.io/)

[Sublime Text 2](http://www.sublimetext.com/)

RStudio

[Marxico](http://maxiang.info/)


RMarkdown: example
========================================================
![R Markdown](http://rmarkdown.rstudio.com/images/markdownChunk.png)


RMarkdown: references
========================================================
[Markdown Syntax (Chinese Version)](http://wowubuntu.com/markdown/)

[R Markdown-Dynamic Documents for R](http://rmarkdown.rstudio.com/)

[Interactive Documents](http://rmarkdown.rstudio.com/authoring_shiny.html)

[Shiny Totutial](http://shiny.rstudio.com/articles/)

[Presentations with ioslides](http://rmarkdown.rstudio.com/ioslides_presentation_format.html)


Thank you!
========================================================
We R together.

![R Club](http://i.imgbox.com/LQr4tQZ5.jpg)

