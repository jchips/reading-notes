# Class 1 notes

The introduction to HTML and JavaScript matters because they are two of the main software developing languages, particularly web development. JavaScript is the main programming language for web developers. Understanding computers is important if we are going to be programming with them.

1. HTTP: The browser sends a HTTP request to the server asking for a copy of the website to display for the client. The data being sent across the client and server is sent across the internet.
2. The browser parses the HTML files first. Then it checks the \<link\> and \<script\> tags in the HTML file to find any CSS and JavaScript.
3. To find images, go to Google Images and find an image. If you don't want it to be copyright, then use the filter and select Creative Commons licenses.
4. A string in JavaScript has quotes around it and a number is just a number. EX:

    * ```let string = "hello world";```
    * ```let num = 5;```

5. Variables are what we use to store values. We can create a variable using the let or const keywords. Variables can make your page dynamic.

Introduction to HTML

1. An HTML attribute is a part of an HTML tag that hold extra info that doesn't appear as content on the page.
2. Under the \<!DOCTYPE html\> tag, you have the \<html\> tags. Inside those goes the \<head\> and the \<body\> tags. In the \<head\> tag goes the metadata and the \<title\> element for the page name. You also put CSS links in the head tag. In the \<body\> tag you put everything that will be displayed on the webpage (so basically everything else).
3. \<article\> tag is for part of a page that can stand by its own (ex: a blog post). The \<section\> tag is for grouping up distinct sections of the content on the page.
4. A typical website includes the following: \<header\>, \<main\>, \<footer\> and maybe a \<nav\> and an \<aside\>.
5. The metadata influences Search Engine Optimization (SEO) by having the ability to make the page appear higher in relevant searches in search engines.
6. To specify metadata there is a name and content attribute for the \<meta\> tag. Using them you can specify what type of meta element you're using and kind of content the meta element contains.

Designing a website

1. First step to designing a website is figure out what you want to accomplish with the site. List the goals you want to reach for the website.
2. The most important to ask yourself when making a website is: What exactly do I want to accomplish?

Semantics

1. You should use \<h1\> for top level heading rather than a \<span\> because the webpage will automatically make the h1 text bigger for you and \<h1\> is a semantic element.
2. Semantic elements have several benefits such as search engines will consider its contents as important keywords in the page's search rankings, screen readers will use to help visually impaired people, and it helps organize the page contents so other developers can read/understand it easier.

JavaScript

1. JavaScript is required to run APIs and to make events (like a click event).
2. To add JavaScript to your page you use \<script\> tags. You can either input code directly in the script tags or use \<script src="js-source"\>\</script\>
