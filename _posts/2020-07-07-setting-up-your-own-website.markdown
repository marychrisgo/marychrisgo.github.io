---
layout: post
title:  "Setting Up Your Website"
date:   2020-07-07 06:56:45 +0800
categories: blog-post
---

<div style="text-align: justify">
There are about 200 million websites up on the internet. A lot of them were built by regular people (non-web developers). I do not have a background in web development, but my internship in Thinking Machines made me study the whole concept in less than two months. 

Luckily, it’s relatively easy and fun to do. I even told my manager this is the kind of job I’m interested in. Thanks to him for pushing me to have my own website. Now, buckle up! I’m gonna help you start your own website too. We’ll go through the steps one by one. 

There are tons of ways to build your own website. A lot of platforms are scattered on the internet making web development easy as 1,2,3! For me, the best way to build your website is through GitHub and Jekyll, especially if you’re just a beginner like me. 

</div>
<br/>

# Steps

1. Make a [GitHub](https://github.com/) account. 
2. Create a new repository.
3. Rename the repository to <username>.github.io
4. Go to Settings, scroll down, select a theme. There are a variety of choices when picking your own theme!
5. You can now check your website at `https://www.<username>.github.io`
6. [Jekyll](https://jekyllrb.com/docs/) is a static-site generator that lets you build your own website with GitHub. If you wanna be fancier, customize Jekyll by setting up the [Ruby environment](https://jekyllrb.com/docs/installation/). There are detailed instructions on the site, and you can choose whatever OS you are using. 
7. After successfully installing Jekyll, run this in your command: <br/>
`jekyll new`
8. Then, time to run your website on localhost:4000! <br/> 
`bundle exec jekyll serve`
9. Voila! Your site is up on your localhost!
10. Connect your local files to your github repo by making a git folder first: <br/> 
`git init`
11. Make a local version of your github repo: <br/> 
`git push origin`
12. If you wanna make changes in the future, make sure you’re local is updated with the remote site by always doing: <br/> 
`git pull  --rebase master.`
13. After updating your local files, you can now make a new branch and push a request to your repository. Since you’re also the admin, pull the request as well. 
14. You can now check your website, the changes should reflect right away! 

This phase is just the starting point! Time to fill up your site with your own content. Good luck!

### **CONTACT ME**

Any questions/feedback/suggestions? Email me. 
