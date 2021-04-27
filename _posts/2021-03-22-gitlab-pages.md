---
layout: single
title:  "Beware of using GitLab pages with a custom domain"
header:
categories: 
tags:
  - website
  - gitlab
---

I set up this page using the [academicpages](https://github.com/academicpages/academicpages.github.io) Jekyll theme. The documention for `academicpages` describes how to set up hosting through GitHub, but I wanted to be able to build the site locally and then build on Git**Lab**, so that I could host the site on GitLab Pages using a custom domain. As I was setting the custom domain on GitLab Pages, I got an error `Domain has already been taken`. It turns out this is a [longstanding issue](https://gitlab.com/gitlab-org/gitlab/-/issues/15921) with GitLab Pages because I had used the domain for another project. Some users mention having to wait weeks/months for encryption certificates to expire and I couldn't find a workaround for GitLab. 

I decided to mirror the repo to GitHub and host from there via GitHub Pages (with my custom domain). It worked immediately. 