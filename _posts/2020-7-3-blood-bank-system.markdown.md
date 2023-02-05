---
layout: post
title:  "Blood Bank Service"
summary: "A proposed system that uses Cloud Computing to provide an online blood bank system."
author: Eman Sami
date: '2020-7-3 21:45:35 +0200'
category: ['Nodejs','Web Development', 'Fullstack']
tags: Node
thumbnail: /assets/img/bbs.png
keywords: Blood bank service, nodejs , express, web development
permalink: /blog/cicd-pipeline/
---

## Features

- Monitoring availability of blood and blood banks among hospitals.
- Requesting blood by individuals, hospitals, clinics, etc. (for short used as
- Individual in Role field for users in website)
- Locating nearest distributer.
- Managing data by admins.
- Adding data by the collectors.
- View and modifying the data by the distributers.
- Database saved on cloud server.


## System Functional Requirements

- The admin should be able to access details of the users
- The admin and the distributers should be able to view and update available blood donations.
- Donors can search for nearby collectors.
- Donors that have already donated in the span of the last three months cannot donate again
and it’s checked by the collectors.
- Donors fill a form to be able to donate.
- Individuals can contact nearby distributers.
- Collectors can add blood donations.
- Individuals fill a form with their requirements.

## Methodology Solution:
By using a REST architectural style which uses HTTP calls for communication
through messages that rely on the HTTP standard: Each request sent by the client through (POST, GET, ... etc.) returns a response
with the required page or action.

The advantage of using REST API is the flexibility it provides by sending different
data based on the calls. This will help with building the website dynamically, and it
can be scaled up.

## Software Requirements:
- HTML, CSS,Javascript
- Bootstrap
- Nodejs, Express
- MongoDB



### Contact us to ask for complete source code! 
<!-- ```yml
Heloo
```

Then to render this category using link and pages. All we need to do is,

1. Create a new file with [your_category_name].md inside categories folder.

2. Copy categories/sample_category.md file and replace the content in [your_category_name].md in that. (Please don't copy the code below its just sample, since it renders the jekyll syntax dynamically) -->

<!-- ```jsx
---
layout: page
title: Guides
permalink: /blog/categories/your_category_name/
---

<h5> Posts by Category : {{ page.title }} </h5>

<div class="card">
{% for post in site.categories.your_category_name %}
 <li class="category-posts"><span>{{ post.date | date_to_string }}</span> &nbsp; <a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</div>
``` -->

<!-- Using the category, all the posts associated with the category will be listed on
`http://localhost:4000/blog/categories/your_category_name` -->