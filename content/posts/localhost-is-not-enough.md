---
title: "Localhost Is Not Enough"
date: 2018-03-04T18:57:33+01:00
draft: false
---

# what happened up till now

So now I got the site running on localhost, but that is not enough.
We want visitors!
So this is the plan:
 [ ] push the hugo site to github in it's own repository
 [ ] create a netlify site
 [ ] let netlify build and deploy

# push the hugo site to github in it's own repository

Quit simple: create an empty repository site-yunus in the already existing github account and set the remote for the local git repository like this

`git remote set-url origin git@github.com:ejpundit/site-yunus.git`

Now upload the ssh key to github to authenticate.
Git push and we are done.

# create a netlify site

Using the existing netlify account it is easy to deploy a new site.
Just select the source, in our case github and select from the found repositories site-yunus.
Ok, everything was working fine, but no posts were found due to a lack of knowledge of hugo.
Hugo differs between draft, expired and future versions. Building with just `hugo` will take draft content into account.
The draft status defaults to true and is set in the frontmatter of the content. Switch it to false et voila ... .

# let netlify build and deploy

Committing automatically starts the build and a successfull build starts automatically the deploy.
So: ![hugo-github-netlify](https://colinwilson.uk/img/hugo-github-netlify.png)






