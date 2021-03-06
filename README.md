# Perchwire

*September 2016*

Earlier this year, I read the 2012 post by Development Seed, titled [How We Build CMS-Free Websites](https://developmentseed.org/blog/2012/07/27/build-cms-free-websites).

> Prose.io and Jekyll enable building simple, flexible, and reliable without the overhead of dynamic CMSs.

> In fact, we’ve deployed most of our projects for free using GitHub Pages, a service that hosts static files directly from a code repository. In more advanced cases, we can deploy sites on Amazon’s S3 service, which provides reliable and scalable static file hosting at high speed and low cost.


I'm building this test website by using Jekyll with GitHub pages, but I'm not using a local install of Jekyll, which requires using git to commit the web posts.

I'm using GitHub's web browser editor to create, update, and commit pages, which should allow me to create and edit posts from any device.


### Initial Steps

I created a new GitHub account with username perchwire.

I followed instructions at <https://github.com/barryclark/jekyll-now> and I forked that repository. Then I changed the name to perchwire.github.io. The repository is helpful for getting started with using Jekyll and GitHub Pages.

The author of the above repository also created this helpful  smashingmagazine.com article titled [Build A Blog With Jekyll And GitHub Pages](https://www.smashingmagazine.com/2014/08/build-blog-jekyll-github-pages).

In addition to using GitHub's web browser editor to maintain content, I'm testing Development Seed's editor called [Prose](http://prose.io), which is designed to work with GitHub Pages by connecting to a GitHub account. It's pretty slick. Well done.

When any file is saved within my GitHub Pages repository (perchwire.github.io), GitHub automatically rebuilds the site, or it rebuilds the changed page.

It only took minutes to create the new GitHub account, fork Barry Clark's repository, and edit the config file to see my new website.



### Custom Domain Name

From the Smashing Magazine article:

> Go to the root of your blog’s repository, and edit the CNAME file to include your domain name (for example, www.yourdomainname.com).

The CNAME file was empty. I added only one line: www.perchwire.com and saved it.

I bought perchwire.com this past summer through my AWS account. I logged into my AWS account and using Route 53, I added the following DNS entry for perchwire.com:

* type = CNAME
* name = www (that was added to perchwire.com.)
* value = perchwire.github.io
* TTL = 300 (the default)

Saved entry. Checked https://www.whatsmydns.net and the info had already propagated. 

Visited http://www.perchwire.com and it worked.

Easy. Fascinating.



### Jekyll Help

* [YAML Front Matter](http://jekyllrb.com/docs/frontmatter)
* [Variables](http://jekyllrb.com/docs/variables)
* [Liquid Templating](https://github.com/Shopify/liquid/wiki)



### Other Forkable Themes

And repositories to view for help.

* <https://github.com/mmistakes/skinny-bones-jekyll>
  * <https://mademistakes.com>
* <https://github.com/mojombo/mojombo.github.io>
  * <http://tom.preston-werner.com>
* <https://github.com/holman/left>
  * <https://zachholman.com>

