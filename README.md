# Team-4795.github.io

## Background

This is the website for the Eastbots robotics team. The website can be found at http://eastbots.com/.

The website is depended upon [Jekyll](https://jekyllrb.com/ "Jekyll
Homepage"). If you are unfamiliar with this and wish to edit, it is
recommended that you familiarize yourself. A working knowledge of
Markdown is required; knowledge of HTML and CSS is also helpful
[Git](https://git-scm.com/ "Git Homepage")
is used for version control.

## Editing Practices

### Images

All images are found in the `assets` folder. When uploading images for
a specific website or blog post, please create a special and clearly
marked folder within `assets`.

To add images to the front page carousel, place them in `assets/carousel`. Amal's wonderful programming will take care of the rest.

### New Pages
To create a new page from the homepage, create a folder with the desired page name and then an `index.md` file within that. This serves to improve organization and clean up URLs. Remember to update `nav.html` when necessary. In the Markdown file, with the Jekyll header should be written as such:

```
---
title: title
layout: examplelayout
---
```

Inside of the `_includes` directory, create a file called `examplelayout.html` and write the page as normal with references to the `index.md` file inlcuded as per [Jekyll syntax](https://jekyllrb.com/docs/home/ "Jekyll Documentation"). Upon building, Jekyll will build the website in the `_site` directory as a combination of these files. **Do not** edit the files in this directory directly unless you are certain of what you are doing.

## Analytics
The website uses Google Analytics to track analytic data.

## Previewing changes on your local machine before committing

### One-time setup

To prepare your local computer for testing the website without doing the git
commit and etc, First install ruby if you don't have it already.
On RHEL/CentOS/Fedora, run this:

	sudo yum install ruby-devel

On Debian/Ubuntu, I think this is right:
	sudo apt-get update
	sudo apt-get install ruby ruby-dev
	
Then following https://jekyllrb.com/resources , run:

	gem install bundler jekyll

also probably required:

	gem install github-pages

### Testing each website change

Before comitting, run this command to build a local copy of the site
and run a local server for testing:

	bundle exec jekyll serve

then point your browser to whatever it says, typically http://localhost:4000

to rebuild site:

	bundle exec jekyll build

to clean up generated files after doing a local build, run

   	bundle exec jekyll clean

