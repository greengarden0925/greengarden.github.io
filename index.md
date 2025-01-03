---
title: "My Book"
author: "Your Name"
output:
  bookdown::bs4_book:
    theme: cosmo
    split_by: section
---

# Preface

Welcome to **My Book**! This is a sample book created using Markdown and rendered with **bookdown**.

In this book, you'll find:

- Easy-to-read chapters.
- Responsive design for any device.
- Navigation-friendly layouts.

# Chapter 1: Introduction

## 1.1 Why Markdown?

Markdown is a lightweight markup language that is:

- Easy to write and read.
- Compatible with many tools.
- Perfect for technical documentation.

## 1.2 Features of `bs4_book`

The `bs4_book` format offers:

- A three-column layout for better navigation.
- Customizable themes via the `bslib` package.
- Mobile-friendly designs.

# Chapter 2: Getting Started

## 2.1 Installation

To get started with **bookdown**, install it in R:

```r
install.packages("bookdown")
```

## 2.2 Rendering Your Book

After setting up your chapters, render the book with:

```r
bookdown::render_book("index.Rmd", "bookdown::bs4_book")
```

This will generate your static site in the `_book` folder.

# Chapter 3: Customization

## 3.1 Themes

You can choose from a variety of themes for your book. For example, in your `_output.yml` file:

```yaml
bookdown::bs4_book:
  theme: flatly
```

## 3.2 Adding CSS

To further customize your book, you can add a `custom.css` file and link it in `_output.yml`:

```yaml
bookdown::bs4_book:
  css: custom.css
