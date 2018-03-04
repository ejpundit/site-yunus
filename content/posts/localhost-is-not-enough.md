---
title: "Localhost Is Not Enough"
date: 2018-03-04T18:57:33+01:00
draft: false
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

Quit simple: create an empty repository site-yunus in the already existing github account and set the remote for the local git repository like this

`git remote set-url origin git@github.com:ejpundit/site-yunus.git`

Now upload the ssh key to github to authenticate.
Git push and we are done.

## create a netlify site


