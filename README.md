# Team-4795.github.io

## Background

This is the website for the Eastbots robotics team. The website can be found at http://eastbots.com/.

The website is depended upon [Jekyll](https://jekyllrb.com/ "Jekyll Homepage"). If you are unfamiliar with this and wish to edit, it is recommended that you familiarize yourself. A working knowledge of HTML, Markdown, and CSS is also necessary. [Git](https://git-scm.com/ "Git Homepage") is used for version control.

## Editing Practices

### Images
All images are found in the `assets` folder. When uploading images for a specific website or blog post, please create a special and clearly marked folder within `assets`.

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