---
layout: post
title:  " To Overcome Challenges, Stop Comparing yourself to Other"
summary: "overcoming comparison to foster personal growth happiness, emphasizing gratitude and self-awareness."
author: Fathima Riham MN
date: '20-10-2021 02:07 +0530'
category: ['Self-Improvement','Mental Health', 'Personal Growth','Positive Thinking']
tags: comparison
thumbnail: /assets/img/posts/code.jpg
keywords: Comparison, Self-worth, Gratitude, Personal Growth, Motivation
usemathjax: false
permalink: /blog/to-overcome-challenges/
---

##  To Overcome Challenges, Stop Comparing yourself to Other 

To add categories in blog posts all you have to do is add a **category** key with category values in frontmatter of the post :

```yml
---
category: ['jekyll', 'guides', 'sample_category']
---
```

Then to render this category using link and pages. All we need to do is,

1. Create a new file with [your_category_name].md inside categories folder.

2. Copy categories/sample_category.md file and replace the content in [your_category_name].md in that. (Please don't copy the code below its just sample, since it renders the jekyll syntax dynamically)

```jsx
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
```

Using the category, all the posts associated with the category will be listed on
`http://localhost:4000/blog/categories/your_category_name`