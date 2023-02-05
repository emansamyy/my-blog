---
layout: post
title:  "CI/CD Pipeline for deploying dynamic Website"
summary: "Multi Author Support allows to create articles with different Authors"
author: Eman Sami
date: '2022-12-14 21:45:35 +0200'
category: ['CICD','Pipeline', 'DevOps']
thumbnail: /assets/img/posts/aws.png
keywords: devlopr jekyll, how to use devlopr, devlopr, how to use devlopr-jekyll, devlopr-jekyll tutorial,best jekyll themes, multi author
usemathjax: true
permalink: /blog/added-multi-author-support/
---

## Now Multiple Authors Can Create Articles:

You can now create or collaborate with multiple authors,Especially when you are working with teams. Each author will have a unique page of her written articles also her profile widget in Articles written by his/her.

For this every Author needs to have a unique username (without space) For eg. If Author is John Doe - the username should be **johndoe** or **john-doe** (without space).This key will be used by devlopr, to fetch individual author's profile pages internally.

### Configuring Authors :

Under _authors folder create a author details file (username.md) with his/her username (as described above). For eg. **johndoe.md**.

Then add this frontmatter to describe the author in **johndoe.md**.
```yml
---

```

Likewise ! This will be helpful for the widgets. (About Author, Recent Articles).

### Adding Author to Post

When creating a new post, just add the author in frontmatter using the username of the author

For eg, In 2020-10-24-demo-article.md
```yml
---
layout: post
title: "Demo Article"
author: janedoe
---
This is Jane Doe's Article
```

Now there will be Authors widget in Blog Sidebar, showing all authors like this :

![Author Sidebar Widget](https://res.cloudinary.com/sujaykundu/image/upload/c_scale,fl_progressive,w_400/v1603700133/3_tiuar0.png)

Also a Author Profile Page will be created for Jane Doe to showcase her written articles.

![Author Page](https://res.cloudinary.com/sujaykundu/image/upload/c_scale,fl_progressive,w_400/v1603643237/1_ee3yke.png)

Also, below this article you can see the Author Profile Card , who has written the article too ! ;)

Cheers ! Hope You enjoy this new feature. :D


