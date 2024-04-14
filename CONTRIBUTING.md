The website is built as a GitHub page. The code for that is available in a GitHub repository on the project's organisational account at:

https://github.com/uk-third-sector-database/uk-third-sector-database.github.io

The website is hosted at http://uk-third-sector-database.io/. This redirects from uk-third-sector-database.github.io via the CNAME file.

To update the website, you will need a GitHub account, and be invited as a collaborator to the GitHub repository which builds the website (or, alternatively, to make a 'fork' and then do a 'pull request').

The website itself is a fork of ['Academic Pages'](https://github.com/academicpages/academicpages.github.io).

If you want to publish a blog post, simply put a new .md file in the _posts repository (i.e. [here](https://github.com/uk-third-sector-database/uk-third-sector-database.github.io/tree/master/_posts). It should begin with a preamble such as:

```
---
title: 'Building a UK Third Sector Database'
date: 2023-01-30
permalink: /posts/2023/001/blog-post-1/
tags:
  - third sector
  - charity data
  - civil society
---
```

To edit the 'Advisory Board' section (which needs updating), you should edit the 'advisory-form.md' file in the '_pages' directory (i.e. [here](https://github.com/uk-third-sector-database/uk-third-sector-database.github.io/blob/master/_pages/advisory-board.md)).

To update the 'Team' section which may or may not be out of date, you should edit the 'meet-the-team.md' file in the '_pages' subdirectory, i.e. [here](http://uk-third-sector-database.io//meet-the-team/).

These should be the three most commonly edited things. If you would like to edit other pages on the site, these can either be found in a subdirectory of the root directory (i.e. './_talks/*' for a subdirectory of talks, or the '_posts' subdirectory, as above), or for pages which don't index multiple things (i.e. an index of blog posts, talks, etc), in the '_pages' subdirectory as above.

Delighted for all/any questions, or for people to raise 'issues' as a mechanism for things they want adding.
