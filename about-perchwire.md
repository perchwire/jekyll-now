---
layout: page
title: About Perchwire
permalink: /about-perchwire/
published: true
---



### August 2018

In late 2016 and early 2017, I made perchwire.com mirror the main website, located at babyutoledo.com. Since the spring of 2017, however, I have not kept up with changes made at babyutoledo.com, which means perchwire.com is no longer a direct mirror, but that's okay. This was only a test or proof-of-concept, and it worked fine, as expected. If necessary, it would be easy to switch the main website away from my setup below to use GitHub Pages.



### September 2016

*Using a static site generator*
 
I'm building this test website perchwire.com by using Jekyll with GitHub Pages, but I'm not using a local install of Jekyll, which requires committing web posts with a local install of git.

No command line actions are requried with this setup. I'm using GitHub's web browser editor to create and update pages.

I created a new GitHub account with username perchwire.

I followed instructions at <https://github.com/barryclark/jekyll-now> and I forked that repository. Then I changed the repo name to perchwire.github.io. The repository is helpful for getting started with using Jekyll and GitHub Pages.

The author of the above repository also created this helpful  smashingmagazine.com article titled [Build A Blog With Jekyll And GitHub Pages](https://www.smashingmagazine.com/2014/08/build-blog-jekyll-github-pages).

In 2016, I drew SSG inspiration by reading this 2012 article by Development Seed, titled [How We Build CMS-Free Websites](https://developmentseed.org/blog/2012/07/27/build-cms-free-websites/).

In addition to using GitHub's web browser editor to maintain content, I'm testing Development Seed's editor called [Prose](http://prose.io), which is designed to work with GitHub Pages by connecting to a GitHub account. I like the editor.

When any file is saved within my GitHub Pages repository (perchwire.github.io), GitHub automatically rebuilds the site, or it rebuilds the changed page.


### Baby University Webstie

In 2014, I created a web publishing app, called Grebe. In 2015, I volunteered to build a website for a local non-profit called Baby University.

I built <http://babyutoledo.com> using my Grebe web publishing app. I can create Grebe posts by using Textile, Markdown/MultiMarkdown, and HTML. The content is stored in a MySQL database, but I cache content in Memcached after creates and updates. When a user clicks a link, the Nginx web server checks Memcached for the cached page. If it's found in Memcached, then my Grebe code is never executed, which means no database access. If the page was not found in Memcached, possibly after flushing the cache for some reason, then Nginx executes my Grebe code, which pulls content from the database, and then Grebe creates the page dynamically by applying the appropriate template. And then the page is stored in Memcached.

Since I've recently taken a liking to the concept of static HTML-based websites, I want to try to recreate much of the Baby U website at perchwire.com, using Jekyll and GitHub Pages. 

I think that search is the only function that requires content to be dynamically-generated for browsing-only users. The blog section at Baby U is dynamically-generated in my Grebe app. The vast majority of the site, however, could be served via static HTML pages.

The customized version of Grebe that I use at Baby U permits using different page templates on a per-post basis. That should be easily replicable with Jekyll.

I have already recreated the Adopt a Family page.

* Perchwire.com + Jekyll + GitHub Pages : [Adopt a Family](http://www.perchwire.com/adopt-a-family/)
* BabyUToledo.com + Grebe : [Adopt a Family](http://babyutoledo.com/4/adopt-a-family)

To-dos as of Sep 17, 2016:

* recreate the look for the default Baby U pages
* recreate the Baby U homepage
