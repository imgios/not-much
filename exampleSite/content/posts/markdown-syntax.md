---
title: "Markdown Syntax Guide"
date: 2024-12-14
slug: "markdown-syntax-guide"
description: "Sample article showcasing basic Markdown syntax and formatting for HTML elements"
keywords: ["gohugo", "hugo", "go", "blog"]
draft: false
tags: ["markdown", "css", "html", "themes"]
math: true
summary: This article offers a sample of basic Markdown syntax that can be used in Hugo content files, also it shows whether basic HTML elements are decorated with CSS in a Hugo theme.
---

This article offers a sample of basic Markdown syntax that can be used in Hugo content files, also it shows whether basic HTML elements are decorated with CSS in a Hugo theme.

## Headings

The following HTML `<h1>`—`<h6>` elements represent six levels of section headings. `<h1>` is the highest section level while `<h6>` is the lowest.

# H1

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas consequat tortor a leo lacinia, non accumsan nisi aliquam. Integer sagittis placerat eros ac venenatis.

## H2

Etiam sem dui, eleifend vel euismod eu, condimentum ac felis. Etiam tellus lectus, maximus nec sollicitudin a, semper sit amet nibh. Vestibulum a sollicitudin augue.

### H3

Donec fermentum tempor sapien, nec lacinia ex condimentum posuere. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis mattis et est sed ornare. Suspendisse auctor arcu ac purus lobortis, vitae accumsan justo eleifend.

#### H4

Maecenas faucibus odio quis molestie accumsan. Ut sit amet purus et justo egestas placerat. Duis vulputate orci pharetra lectus congue placerat. Curabitur egestas tempor quam, a elementum nibh molestie nec. Vestibulum dignissim justo vehicula augue laoreet, at vehicula enim vulputate.

##### H5

Vestibulum accumsan, sapien ut sollicitudin condimentum, libero purus vulputate nisl, id aliquet turpis ipsum eu justo. Proin aliquam, massa sit amet mattis hendrerit, diam nisl dictum sem, quis accumsan sapien elit ac augue. Nunc tincidunt velit eget lorem rutrum, ac congue mauris eleifend.

###### H6

onec et vestibulum quam. Mauris fermentum enim nibh, sit amet commodo quam ornare nec. Maecenas sed pellentesque nisl, at gravida sapien. Nam non enim id quam malesuada suscipit ut eget nisi.

## Paragraph

Xerum, quo qui aut unt expliquam qui dolut labo. Aque venitatiusda cum, voluptionse latur sitiae dolessi aut parist aut dollo enim qui voluptate ma dolestendit peritin re plis aut quas inctum laceat est volestemque commosa as cus endigna tectur, offic to cor sequas etum rerum idem sintibus eiur? Quianimin porecus evelectur, cum que nis nust voloribus ratem aut omnimi, sitatur? Quiatem. Nam, omnis sum am facea corem alique molestrunt et eos evelece arcillit ut aut eos eos nus, sin conecerem erum fuga. Ri oditatquam, ad quibus unda veliamenimin cusam et facea ipsamus es exerum sitate dolores editium rerore eost, temped molorro ratiae volorro te reribus dolorer sperchicium faceata tiustia prat.

Itatur? Quiatae cullecum rem ent aut odis in re eossequodi nonsequ idebis ne sapicia is sinveli squiatum, core et que aut hariosam ex eat.

## Footnotes

Here's a simple footnote[^1], and here's a longer one[^bignote].

[^1]: This is the first footnote.

[^bignote]: Here's one with multiple paragraphs and code.

    Indent paragraphs to include them in the footnote.

    `{ my code }`

    Add as many paragraphs as you like.

Code:

```md
Here's a simple footnote,[^1] and here's a longer one.[^bignote]

[^1]: This is the first footnote.

[^bignote]: Here's one with multiple paragraphs and code.

    Indent paragraphs to include them in the footnote.

    `{ my code }`

    Add as many paragraphs as you like.
```

## Blockquotes

The blockquote element represents content that is quoted from another source, optionally with a citation which must be within a `footer` or `cite` element, and optionally with in-line changes such as annotations and abbreviations.

#### Blockquote without attribution

> Tiam, ad mint andaepu dandae nostion secatur sequo quae.
> **Note** that you can use _Markdown syntax_ within a blockquote.

#### Blockquote with attribution

> Don't communicate by sharing memory, share memory by communicating.
>
> — <cite>Rob Pike[^1]</cite>

[^1]: The above quote is excerpted from Rob Pike's [talk](https://www.youtube.com/watch?v=PAAkCSZUG1c) during Gopherfest, November 18, 2015.

## Tables

Tables aren't part of the core Markdown spec, but Hugo supports them out-of-the-box.

| Text aligned on the left  | Text aligned in the center | Text aligned on the right |
| ----- | :---: | ----: |
| left   | center  | right |
| left   | center  | right |
| left   | center  | right |
| left   | center  | right |

#### Inline Markdown within tables

| Inline style | Rendered |
| --------- | -------- |
| `_italics_` | _italics_ |
| `**strong**` | **strong** |
| ``code`` | `code` |
| `~~strikethrough~~` | ~~strikethrough~~ |
| `$\varphi = \dfrac{1+\sqrt5}{2}= 1.6180339887…$` | $\varphi = \dfrac{1+\sqrt5}{2}= 1.6180339887…$ |
| `[Link](https://example.com)` | [Link](https://example.com) |
| `[Link](https://example.com "Example link with tooltip")` | [Link with tooltip](https://example.com "Example link with tooltip") |

## List Types

#### Ordered List

1. First item
2. Second item
3. Third item

#### Unordered List

- List item
- Another item
- And another item

#### Nested Unordered list

- Fruit
  - Apple
  - Orange
  - Banana
- Dairy
  - Milk
  - Cheese

#### Nested Ordered list

1. Fruit
    - Apple
    - Orange
    - Banana
2. Dairy
    1. Milk
    2. Cheese
3. Third item
    1. Sub One
    2. Sub Two

#### Definition List

First Term
: This is the definition of the first term.

Second Term
: This is one definition of the second term.
: This is another definition of the second term.

#### Task list

- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media

## Other Elements — abbr, sub, sup, kbd, mark

<abbr title="Graphics Interchange Format">GIF</abbr> is a bitmap image format.

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

Press <kbd><kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>Delete</kbd></kbd> to end the session.

Most <mark>salamanders</mark> are nocturnal, and hunt for insects, worms, and other small creatures.