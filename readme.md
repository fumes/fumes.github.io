## What?

_Fumes is an online photography magazine broadcasting human interest stories mainly from South East Asia.__Fumes project was started by two photographers. A metaphor to play with, delivering ideas via images._

♡ Fumes website is now refactored.  

☯ Articles are structured as `photographer`|`curator` symbiotic work.  

✿ This will bloom greener fumes soon...## Structure

- Now using the [Source branch](https://github.com/fumes/fumes.github.io/tree/source) for development which is then deployed automagically to Netlify CDN at every update.

- 'Master branch' is redundant now. It's just the locally compiled ```_site``` folder pushed via rake script (not useful, just a compiled copy without source files... just an exercise, might even delete it someday!)

- More **working branches** maybe present at times...

## Fumes website features

- [x] microformats. [example test here](https://search.google.com/structured-data/testing-tool#url=http%3A%2F%2Ffumes.junglestar.org%2Fstudies%2Fform)

- [x] serious, maybe dated,  [responsive](https://github.com/wildlyinaccurate/jekyll-responsive-image) [image](https://github.com/BBC-News/Imager.js/).  

- [x] ultra simple [codepen-geek](http://codepen.io/rokma/full/pJBXbg/) responsive logo.  

- [x] smart [inline svg icons](https://github.com/eduardoboucas/eduardoboucas.github.io/tree/master/_includes/svg).  

- [x] auto [tag](http://geoexamples.com/other/2015/06/04/Jekyll-tags-plugin-gh-pages.html) navigation.  

- [x] auto [category](http://geoexamples.com/other/2015/06/04/Jekyll-tags-plugin-gh-pages.html) navigation.  

- [x] post thumbs. Front-matter declared.  

- [x] chrome standalone web app functionality (android only :().  

- [x] photographer indexes and navigation.   

- [x] open graph.  

- [x] attribution footnotes ["APPEND to copy action"](https://www.jitbit.com/alexblog/230-javascript-injecting-extra-info-to-copy-pasted-text/) via inlined vanilla js.  

- [x] twitter [cards](https://github.com/merlos/jekyll-auto-image#example-using-twitter-cards) ([tested here..](https://cards-dev.twitter.com/validator)).   - [x] handy prev-next articles navigation.

- [x] SSL/https thanks to Netlify.

- [x] responsive videos without plugins thanks to [eduardo boucas](https://eduardoboucas.com/blog/2016/12/21/responsive-video-embeds-jekyll.html)

- [x] Reading time estimates. Using this gem [liquid_reading_time](https://github.com/bdesham/reading_time)


Not yet:

- [ ] print.css  

- [ ] [google authors](http://milanaryal.com/2015/integrating-social-meta-tags-into-jekyll/#integrating-google-authorship-into-jekyll)  

- [ ] [Google Author Rich Snippets](http://davidensinger.com/2013/05/setting-up-google-author-rich-snippets/)  

- [ ] service workers.


### Fumes development technologies

Stuff for development. Its happens in [Source branch](https://github.com/fumes/fumes.github.io/tree/source):

- Nmp

- Gulp

- Bundler

- plus various code clips & techniques taken here and there...  

- Netlify CND and SSL/https.


#### Prerequisites, first setup:

##### A. Get started with bundler. Install it globally!

```sh
gem install bundler```

##### B. Install gulp globally

```sh
npm install --global gulp
```

#### Dev prerequisites:

##### 3. cd into local project's dir

```sh
cdf
```
##### 2. Install gems dependencies into project's local dir

```sh
bundle install
```

##### 1. Install node dependencies into project's local dir

```sh
npm install
```

#### Dev time:

##### 0. cd in local project dir

```sh
cdf
```

##### 1. Run Jekyll

```sh
bundle exec jekyll serve
```

##### 2. Run gulp (optional)

Open a new terminal window and

```sh
gulp
```

#### Gems dependencies:

- gem 'rake'

- gem 'rmagick'

- gem 'jekyll', '3.0.1'

- gem 'jekyll-sitemap'

- gem 'liquid_reading_time'

- gem ['jekyll-responsive_image'](https://github.com/wildlyinaccurate/jekyll-responsive-image)### Plugins dependencies:

- [categories_generator.rb](http://geoexamples.com/other/2015/06/04/Jekyll-tags-plugin-gh-pages.html)

- [tags_generator.rb](http://geoexamples.com/other/2015/06/04/Jekyll-tags-plugin-gh-pages.html)

- [responsive_image.rb](https://github.com/wildlyinaccurate/jekyll-responsive-image)

- [imager.js](https://github.com/BBC-News/Imager.js/)### More credits- [github setup tips](http://ixti.net/software/2013/01/28/using-jekyll-plugins-on-github-pages.html)## To do##### Urgent:- [ ] licenses management: use licenses.yml- [ ] icons slim diet- [ ] publish some content!##### Sometime soon:- [ ] get rid of jquery- [ ] refactor using Imager.js + gulp grinder, drop responsive_image.rb- [ ] compress html##### One day:- [ ] install service workers- [ ] disqus- [ ] print.css- [ ] mailchimp- [ ] merchandise- [ ] PDF | ebook

## Purpose of open sourcing this project

Having the source files of the Fumes project website, the core of the project, out in the open will allow other people or organizations that want to produce journalism to get a head-start on their own sites and see some practices and methods that have worked well for Fumes.

## Reasons for using Jekyll (or any other static site generator)

This project creates static HTML files using [Jekyll](http://jekyllrb.com/). There are many main reasons for using a static site generator this way:

1. The site will hold up to **high load** without requiring any special caching techniques. It's just HTML.

2. Since the site is just static files without a CMS it **can sit for years without needing any software updates or security patches**, which is important for reference websites like Fumes that will sit without content changes for a long time.

3. Since it's all text files controlled by a Git repository, **collaboration is made easy.**

4. **Stories can be produced extremely quickly.** To produce the stories, just edit text files. A huge speed-up. With a little Markdown learning, everybody can quickly achieve full proficiency. Jekyll allows for include files, which separate content from presentation thus allows for changing already placed elements —like side images, interactives, etc.— without changing the story page. Huge speed-up during crunch time.

5. **Fast and Secure.** All static files so drastically reduced vulnerabilities compared to popular php CMS like WP.

6. Hosted on github pages. World class hosting on cdn for sharing.


## Warning

Despite this repo being public, it doesn't mean that all these assets are open-source and/or copyright free, or even that you may use any of them.

Please, ask for permission first by contacting us: [_info@junglestar.org_](mailto:info@junglestar.org)

Thanks, Junglestar team.

## Photo rights

All photos © the Authors. All photos rights reserved. Except as indicated on a per article basis.  

In some Fumes Articles, photos are released under CC-BY Creative Commons license. Some other fumes photos are CC0. Everything else is GPL.
