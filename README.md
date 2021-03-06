# saskblockchain.ca
saskblockchain.ca website

Static website generated by [Hugo](https://gohugo.io).

Site content is located in the `content` directory.  Templating is in `layouts`, using Bootstrap CSS.


## Local development

1. Install Hugo
2. Fork this repo
3. Clone your fork
4. Run `hugo serve`
5. Open website at [http://localhost:1313](http://localhost:1313)
6. Create new content:  
  * New news item: `hugo new news/<post name>.md`
  * New event: `hugo new events/<event name>.md`
7. Commit changes
8. Submit pull request


Commits to `master` trigger a Github action that rebuilds the static html files and deploys to [https://github.com/sask-blockchain/sask-blockchain.github.io](https://github.com/sask-blockchain/sask-blockchain.github.io)

### Page front matter

Front matter is meta data included at the top of a content Markdown file.
For example:

```
---
title: "Page title"
slug: page-title
date: 2020-01-03T09:28:33-06:00
tags: [announcement,foo,bar]
homepage: true
---

Page content here...
```

In addition to the [predefined front matter variables](https://gohugo.io/content-management/front-matter/#front-matter-variables)
the follow variables may be included:

| Name | Description |
|------|-------------|
| homepage | If set to `true`, a summary of the article is included on the homepage |


Events have the following additional variables:

| Name | Description |
|------|-------------|
| eventDate | date of the event |
| eventLocation | location of the event |
| eventURL | URL to external event page |
