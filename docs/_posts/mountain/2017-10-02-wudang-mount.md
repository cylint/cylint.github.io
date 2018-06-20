---
layout: post
title: "武当山"
excerpt: "An article to test overriding the default site author."
categories: stories
tags: [武当山, 旅行]
hidelogo: true
image:
  feature: /header/wudang-1.jpg
  credit: WeGraphics
  creditlink: wegraphics.net/downloads/free-ultimate-blurred-background-pack/
---

For those of you who may have content written by multiple authors on your site you can now assign different authors to each post if desired.

Previously the theme used a global author for the entire site and those attributes would be used in all bylines, social networking links, Twitter Card attribution, and Google Authorship. These `owner` variables were defined in `config.yml`

Start by modifying or creating a new `authors.yml` file in the `_data` folder and add your authors using the following format.

```yaml
# Authors

Author1:
  name: Author1
  web: 
  email: 
  bio: 
  avatar: bio-photo.jpg
  twitter: 
  google:
    plus:

    
Author2:
  name: Author2
  web: 
  email: 
  bio: 
  avatar: bio-photo-2.jpg
  twitter: 
  google:
    plus:
```

To assign Author2 as an author for our post. You'd add the following YAML front matter to a post:

```yaml
author: Author2
```
