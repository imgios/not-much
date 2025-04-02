---
title: "Hugo shortcodes"
description: Here is a demo of all shortcodes available in Hugo.
date: 2024-12-27
lastmod: 2025-04-02
keywords: ["gohugo", "hugo", "go", "blog"]
tags: ["hugo", "themes"]
summary: This post shows the default Hugo shortcodes and how they are rendered.
toc: true
---

## Details

{{< details summary="See the details" >}}
This is a **bold** word.
{{< /details >}}

## Highlight

{{< highlight go-html-template >}}
{{ range .Pages }}
  <h2><a href="{{ .RelPermalink }}">{{ .LinkTitle }}</a></h2>
{{ end }}
{{< /highlight >}}

## Images

{{< figure src="https://images.unsplash.com/photo-1560032779-0a8809186efd?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1350&q=80" title="Dave Herring" >}}

{{< figure src="https://images.unsplash.com/photo-1560032779-0a8809186efd?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=80" title="Dave Herring" >}}


## Github Gist

{{< gist imgios f587d813ec6c851d700054f89230fb42 >}}

## Youtube video

{{< youtube w7Ft2ymGmfc >}}

## Tweet

{{< tweet user="GoHugoIO" id="877500564405444608" >}}

## Vimeo

{{< vimeo id="146022717" >}}

## Instagram

{{< instagram BWNjjyYFxVx >}}