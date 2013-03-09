---
layout: page
title: Hello World!
tagline:
---
{% include JB/setup %}

##### Update Author Attributes

In `_config.yml` remember to specify your own data:
{% highlight java linenos=table %}
title : My Blog =)

author :
name : Name Lastname
email : blah@email.test
github : username
twitter : username
{% endhighlight %}

The theme should reference these variables whenever needed.
    
##### Sample Posts

This blog contains sample posts which help stage pages and blog data.
When you don't need the samples anymore just delete the `_posts/core-samples` folder.

Here's a sample "posts list".

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>



