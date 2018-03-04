---
title: "Localhost Is Not Enough"
date: 2018-03-04T18:57:33+01:00
draft: true
---

# `localhost` ist not enough

So now I got the site running on localhost, but that is not enough.
We want visitors!
So this is the plan:
 [ ] push the hugo site to github in it's own repository
 [ ] create a netlify site
 [ ] hook the git repository to netlify
 [ ] configure the build on netlify
 [ ] let netlify build and deploy

 ## push the hugo site to github in it's own repository

 git remote add origin https://github.com/ejpundit/site-yunus.git
 git push -u origin master