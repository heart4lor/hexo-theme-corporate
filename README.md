# Hexo Corporate

Hexo Corporate is a full-featured Hexo theme based on the Metronic Corporate
Frontend freebie framework.  Live example available
[here](http://hexotest.computerlab.io).

This theme is useful for companies interested in using Hexo to create a
professional website with an attractive landing page, company blog, contact
information, and portfolio.  

**Features:**

- custom landing page / index 
- blog posts with tags and categories
- project portfolio
- contact form with google maps
- about page
- swiftype (search) integration
- multiple color schemes
- disqus integration
- social links
- metronic css framework components


## Install

``` bash
git clone https://github.com/ptsteadman/hexo-theme-corporate.git themes/corporate
```

## Enable

1. **Add example pages.** 

	Copy all of the contents of `themes/corporate/_source` to `_source`.
	This includes a sample landing page and contact, project, and
	about pages.

	```bash
	cp -r themes/corporate/_source/* source
	```

2. **Enable theme.** 
	Modify the root site `_config.yml` so that `theme` is set to `corporate`. 

	```yml
	# Extensions
	## Plugins: http://hexo.io/plugins/
	## Themes: http://hexo.io/themes/
	theme: corporate # change this

	```

	Finally, run `npm install` and then `hexo server` to test out the site.

3. **Optional: Enable custom landing page.**

	To use custom landing page instead of the default archive index, remove
	the line containing hexo-generator-index from package.json in the project root.
	Then, edit `source/index.ejs`.

### Update

``` bash
cd themes/corporate
git pull
```

## Configure

Edit `themes/corporate/_config.yml` for theme-specific configuration.

``` yml
# Header Menu
menu:
  Home: /
  Projects: /projects/
  Blog: /archives/ # can set archive-dir in root config to custom value
  Contact: /contact/
  About: /about/
   
rss: /atom.xml

# Content
excerpt_link: Read More
fancybox: true # whether or not to load the fancybox library

# Integrations
disqus_shortname: 
google_analytics:
swiftype_install_key: 

# Social
social:
  github: https://github.com/ptsteadman
  twitter: https://twitter.com/ptsteadman
  facebook: https://www.facebook.com/ptsteadman
  rss: atom.xml
  linkedin: https://linkedin.com/in/ptsteadman
  stackoverflow: http://stackoverflow.com/users/2480493/patrick-steadman

# Miscellaneous
color_scheme: red   # options: blue, gray, green, orange, red, turquoise
favicon: /favicon.ico # path from root of hexo site
twitter_widget_id: "678830341331820544" # as a string, from https://twitter.com/settings/widgets
twitter_username: computerlab_ # twitter username without the @
default_author: Anonymous

about: Computer Lab is a software development and marketing company based in Brooklyn, New York. <br><br> Computer Lab was founded in 2015, and is focused on so on and so forth.
phone: 716-472-4484
email: ptsteadman@gmail.com
address_1: 140 Metropolitan Avenue
address_2: 5th Floor
address_3: Brooklyn, NY 11249
skype: ptsteadman
lat: 40.715911 
long: -73.962147
```


## Features

### Fancybox

Hexo Corporate uses [Fancybox] to showcase your photos. You can use Markdown syntax or fancybox tag plugin to add your photos.

```
![img caption](img url)

{% fancybox img_url [img_thumbnail] [img_caption] %}
```

### Pages

### Swiftype

### Thumbnail

### Featured Posts

### Authors

### Projects

### Color Schemes

## Metronic Freebie License

The Metronic CSS and JavaScript components are included with the following
license:

```
You are free to use this freebie theme in your any personal or commercial
projects. All used resources, plugins, stock images are subject to thier own
licenses!

The only limitation is that you are not permitted to use this theme in a stock
items that sold in any theme marketplaces(e.g: themeforest.net,
wrapbootstrap.com, etc...).
```

## Development

### Requirements

- Hexo 3.0

### Links

