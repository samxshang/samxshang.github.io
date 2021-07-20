---
title: "How I built my website"
permalink: /resources/my-website/
last_modified_at: 2021-07-20T14:00:02-04:00
categories:
  - resource
tags:
  - website
  - skill
---

# ver. 0.1 The website was born

## Initiating the website
The website is hosted by [GitHub Pages][github-pages], and is powered by [Jekyll][jekyll] & [Minimal Mistakes][minimal-mistakes].

[github-pages]: https://pages.github.com/
[jekyll]: https://jekyllrb.com/
[minimal-mistakes]: https://mademistakes.com/work/minimal-mistakes-jekyll-theme/

First, I created a GitHub Pages repository to host my website: `USERNAME.github.io`

Second, I found the free website theme on [Jekyll Themes](https://jekyllthemes.io/).

Third, I downloaded the theme files, and uploaded the files to my repository. Then I published my site. Voila! I've got a website up and running!

## Configuration and settings
Then, I made changes to the settings and personalized my site.

1. \\_root\\_config.yml
2. \\_data\\navigation.yml

## Content
Add a new post: 
name it `YYYY-MM-DD-name-of-post.md`

Front Matter settings:
```yaml
---
title: "Title of the post"
date: 2021-07-19T22:00:02-04:00
last_modified_at: 2021-07-20T16:00:02-04:00
excerpt_separator: "<!--more-->"
categories:
   - blog
   - resource
   - journey
tags:
   - website
   - skill
   - stats
   - r
   - academia
   - research
   - conference
   - paper
   - job
link: https://duckduckgo.com/
---

```

Handy functions:
```html
> Quote something.
  
> <cite><a href="https://duckduckgo.com/">Link to the site</a></cite>
```

> Quote something.
  
> <cite><a href="https://duckduckgo.com/">Link to the site</a></cite>


Kramdown `{: .notice}` : can be added after a sentence as a new line

**Light Grey Notice:** `{: .notice}`
{: .notice}

**Grey Notice:** `{: .notice--primary}`
{: .notice--primary}

**Blue Notice:** `{: .notice--info}`
{: .notice--info}

**Orange Notice:** `{: .notice--warning}`
{: .notice--warning}

**Red Notice:** `{: .notice--danger}`
{: .notice--danger}

**Green Notice:** `{: .notice--success}`
{: .notice--success}

Wrap several paragraphs or other elements in a notice:

```html
{% raw %}{% capture notice-2 %}
#### New Site Features

* You can now have cover images on blog pages
* Drafts will now auto-save while writing
{% endcapture %}{% endraw %}

<div class="notice">{% raw %}
  {{ notice-2 | markdownify }}
{% endraw %}</div>
```

## Learning
1. [Docs-start guide](https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/)
2. [Docs-pages](https://mmistakes.github.io/minimal-mistakes/docs/pages/)
3. [About-notable features](https://mmistakes.github.io/minimal-mistakes/about/#notable-features)
