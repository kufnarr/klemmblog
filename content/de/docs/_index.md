---
title: "Meine Doku Übersicht"
---
Hier steht jetzt endlich mein Text, der hoffentlich erscheint!

## Überschrift

jdölfjdd

## bittebite

="{{ .Site.LanguageCode | default `en-US` }}">

<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="description" content="{{ .Page.Params.description | default .Site.Params.
description | .RenderString }}">
  <meta name="author" content="{{ .Site.Params.author.name }}">
  <meta name="theme-color" content="{{ .Site.Params.project.themeColor.light }}" media=
"(prefers-color-scheme: light)">
  <meta name="theme-color" content="{{ .Site.Params.project.themeColor.dark }}" media="
(prefers-color-scheme: dark)">
  {{ with .Params.robots -}}
  <meta name="robots" content="{{ . }}">
  {{ end -}}

  <title>{{ .Title | .RenderString }} · {{ .Site.Title | .RenderString }}</title>
  <link rel="canonical" href="{{ .Permalink }}">

  {{- $css := slice (resources.Get "css/reset.css") (resources.Get "css/theme.css") (re
sources.Get "css/_btn.css") (resources.Get "css/_select.css") (resources.Get "css/docs.
css") (resources.Get "css/docs-article.css") (resources.Get "css/docs-chroma.css") (res
ources.Get "css/docs-shortcodes.css") | resources.Concat "assets/css/docs.css" | minify
 | fingerprint }}
  <link rel="stylesheet" href="{{ $css.RelPermalink }}" integrity="{{ $css.Data.integri
ty }}">

  {{ partial "favicons.html" . }}
  {{ partial "analytics.html" . }}
  {{ partial "og-x-seo.html" . }}
</head>

<body>

## öjfdlkgjflkjggf
