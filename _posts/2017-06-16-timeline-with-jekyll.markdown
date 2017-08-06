---
title: Timeline with Jekyll
date: 2017-06-16 08:00:00 Z
categories:
- jekyll
- english
- html
- open-source
- project
- theme
images:
- https://raw.githubusercontent.com/lukas-h/jekyll-timeline/master/screenshot.png
- https://raw.githubusercontent.com/lukas-h/jekyll-timeline/master/screenshot2.png
---

[GITHUB PROJECT](https://github.com/lukas-h/jekyll-timeline)

Visualize time structured data with this simple jekyll-template.
This Jekyll site is perfect for your résumé or other timelines.

**how to use it?**
1. Fork the repository [github.com/lukas-h/jekyll-timeline](https://github.com/lukas-h/jekyll-timeline)
2. Configure Github-Pages in the Repo Settings
3. Edit the Markdown files in the collection `steps` in the `_steps` folder  
    
    Required data fields in the frontmatter:
    
    - `title: <TITLE>`
    - `date: 2016-09-31 00:00:00 -0700` (Only Year and Month are shown)

    Optional fields:

    - `enddate: 2017-1-1 00:00:00 -0700`
4. Change site configuration `_config.yml`

    - the Site title: `title`
    - background color `color`
    - url (*important*) `url`
    - baseurl (*important*) `baseurl` (name it after the repo)
    - site's `description`
5. You're done! (Look at https://<*USERNAME*>.github.io/<*REPO*>)

Feel free to contribute, give feedback, a star, and share it!