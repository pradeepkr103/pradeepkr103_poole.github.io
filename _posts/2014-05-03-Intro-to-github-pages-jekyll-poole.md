---
layout: post
title: About Github pages, What's Jekyll and Poole?
---

## Quickstart .. 

* Also being a RoR developer .. I also did the (optional) 
	$ gem install jekyll
	$ jekyll serve
	# Open http://localhost:4000 in your browser, and voilà. You're done.

## About Github pages 

* [see here for getting started](pages.github.com)
	- You get one site per GitHub account and organization, and unlimited project-specific sites.
	- YOU CAN Overwrite with github's automatic page generator.
		Author your content in our markdown editor, select a theme, then publish. 
	- tips: [Create your own Github pages repo](help.github.com/articles/create-a-repo)

* Why Poole? I followed instructions [Joshua](http://joshualande.com/jekyll-github-pages-poole/) and instead of reading a lot of jekyll documentation, I followed HIS instructions using a great git repo called poole that comes with styling, etc. I cheatsheated his cheatsheet. Benefits are :

	- Code examples to be very nicely embedded in the website
	- Ready to go with example templates, pages, posts, and styles
	- Comes with a minimal,decent styling with Hyde (at least for progammers :)
	- You don't need a web server or hosting plan ($50-$100/yr saving!)
	- Discus commenting
	- Use GitHub's web editor to (edit markdown git src) write blog posts online
	- Custom domain it eg. blog.gomobilefirst.com.

* For More reading
	- Poole repo - https://github.com/poole/poole
	- Github pages articles https://help.github.com/articles/
	- http://jekyllbootstrap.com/
	- http://jekyllrb.com/


# About Jekyll

[Jekyll](http://jekyllrb.com) is a static site generator, an open-source tool for creating simple yet powerful websites of all shapes and sizes. From [the project's readme](https://github.com/jekyll/jekyll/blob/master/README.markdown):

> Jekyll is a simple, blog aware, static site generator. It takes a template directory [...] and spits out a complete, static website suitable for serving with Apache or your favorite web server. This is also the engine behind GitHub Pages, which you can use to host your project’s page or blog right here from GitHub.

It's an immensely useful tool. Find out more by [visiting the project on GitHub](https://github.com/jekyll/jekyll).


### Jekyll Blog : Local development, testing

* _site/ If you are NOT using github, you need to run Jekyll yourself. When you run Jekyll, it creates a folder called _site with the static website inside of it. Every file or folder in the repo will get copied into the _site folder unless it begins with an underscore.

* _posts/ The folder _posts contains all of the blog posts in markdown format. 
	$ ls -1 _posts/
	2013-12-31-whats-jekyll.md
	2014-01-01-example-content.md
	2014-01-02-introducing-poole.md


## Poole is Coole

Poole is the butler for [Jekyll](http://jekyllrb.com), the static site generator. It's designed and developed by [@mdo](https://twitter.com/mdo) to provide a clear and concise foundational setup for any Jekyll site. It does so by furnishing a full vanilla Jekyll install with example templates, pages, posts, and styles.


### Options

Poole includes some customizable options, typically applied via classes on the `<body>` element.


### Rems, `font-size`, and scaling

Poole is built almost entirely with `rem`s (instead of pixels). `rem`s are like `em`s, but instead of building on the immediate parent's `font-size`, they build on the root element, `<html>`.

By default, we use the following:

```css
html {
  font-size: 16px;
  line-height: 1.5;
}
@media (min-width: 38em) {
  html {
    font-size: 20px;
  }
}

```

To easily scale your site's typography and components, simply customize the base `font-size`s here.

There are currently two official themes built on Poole:

* [Hyde](http://hyde.getpoole.com)
* [Lanyon](http://lanyon.getpoole.com)

Individual theme feedback and bug reports should be submitted to the theme's individual repository.

### Kudos to Poole!

![Poole](https://f.cloud.github.com/assets/98681/1834359/71ae4048-73db-11e3-9a3c-df38eb170537.png)

See Poole in action with [the demo site](http://demo.getpoole.com).
SRC: github.com/Poole

**Poole's Author is Mark Otto**
- <https://github.com/mdo>
- <https://twitter.com/mdo>

Open sourced under the [MIT license](LICENSE.md).


** What's included **

Poole is a streamlined Jekyll site designed and built as a foundation for building more meaningful themes. Poole, and every theme built on it, includes the following:

* Complete Jekyll setup included (layouts, config, [404](/404.html), [RSS feed](/atom.xml), posts, and [example page](/about))
* Mobile friendly design and development
* Easily scalable text and component sizing with `rem` units in the CSS
* Support for a wide gamut of HTML elements
* Related posts (time-based, because Jekyll) below each post
* Syntax highlighting, courtesy Pygments (the Python-based code snippet highlighter)

Additional features are available in individual themes.

** Limitations** 
1. Poole and it's themes are by preference a forward-thinking project. In addition to the latest versions of Chrome, Safari (mobile and desktop), and Firefox, it is only compatible with Internet Explorer 9 and above.

## Running Local Sites with Jekyll/Pool

### 1. Install Jekyll

Poole is built for use with Jekyll, so naturally you'll need to install that. On Macs, it's rather straightforward:

```bash
$ gem install jekyll
```

**Windows users:** Windows users have a bit more work to do, but luckily [@juthilo](https://github.com/juthilo) has your back with his [Run Jekyll on Windows](https://github.com/juthilo/run-jekyll-on-windows) guide.

You may also need to install Pygments, the Python syntax highlighter for code snippets that plays nicely with Jekyll. Read more about this [in the Jekyll docs](http://jekyllrb.com/docs/templates/#code_snippet_highlighting).

### 2a. Quick start

To help anyone with any level of familiarity with Jekyll quickly get started, Poole includes everything you need for a basic Jekyll site. To that end, just download Poole and start up Jekyll.

### 2b. Roll your own Jekyll site

Folks wishing to use Jekyll's templates and styles can do so with a little bit of manual labor. Download Poole and then copy what you need (likely `_layouts/`, `*.html` files, `atom.xml` for RSS, and `public/` for CSS, JS, etc.).

### 3. Running locally

To see your Jekyll site with Poole applied, start a Jekyll server. In Terminal, from `/Poole` (or whatever your Jekyll site's root directory is named):

```bash
$ jekyll serve
```

Open <http://localhost:4000> in your browser, and voilà. You're done.



