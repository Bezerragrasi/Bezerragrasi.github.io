---
layout: page-fullwidth
permalink: /publication/
title: "Publications"
---
<!-- This page is automatically generated using entries from the file "_data/publications.yml" 
     Please use the file "_data/publications.yml" to include new items.
-->

<!-- To change the list layout go to "_sass/_09_elements.scss 
     under the /* Publication list style */ header  (.publication css class)
-->

<div class="panel radius" markdown="1">
**Table of Contents**
{: #toc }
*  TOC
{:toc}
</div>

## Peer-Reviewed Journal Articles

<!-- Automatically imports class "peer-reviewed" items from file _data/publications.yml -->
<ul class="publication">
    {% for item in site.data.publications %}
    {% if item.class == "peer-reviewed" %}
    <li> {{ item.authors }} ({{ item.year }})
        <a href="{{ item.doi }}">{{ item.title }}</a>.
        <i>{{ item.journal }}</i>
        {{ item.volume }}{% if item.number %}({{ item.number }}){% endif %}: {{ item.pages }}.
    </li>
    {% endif %}
    {% endfor %}
</ul>
{% include _small-top-button.html %}

## Accepted for Publication

<ul class="publication">
    {% for item in site.data.publications %}
    {% if item.class == "accepted" %}
    <li> {{ item.authors }} ({{ item.year }}) {{ item.title }}. <i>{{ item.journal }}</i>.</li>
    {% endif %}
    {% endfor %}
</ul>
{% include _small-top-button.html %}

<!-- ## Under Review

<ul class="publication">
    {% for item in site.data.publications %}
    {% if item.class == "under-review" %}
    <li> {{ item.authors }} ({{ item.year }})
        <a href="{{ item.doi }}">{{ item.title }}</a>.
        <i>{{ item.journal }}</i>.
    </li>
    {% endif %}
    {% endfor %}
</ul>
{% include _small-top-button.html %}

## PhD Thesis

<ul class="publication">
    {% for item in site.data.publications %}
    {% if item.class == "thesis" %}
    <li> {{ item.authors }} ({{ item.year }})
        <a href="{{ item.doi }}">{{ item.title }}</a>.
        <i>{{ item.institution }}</i>, {{ item.address }}.
    </li>
    {% endif %}
    {% endfor %}
</ul>
{% include _small-top-button.html %} -->



## Book Chapters

<ul class="publication">
    {% for item in site.data.publications %}
    {% if item.class == "book" %}
    <li> {{ item.authors }} ({{ item.year }})
        <a href="{{ item.doi }}">{{ item.title }}</a>.
        In: <i>{{ item.journal }}</i>.
    </li>
    {% endif %}
    {% endfor %}
</ul>
{% include _small-top-button.html %}

## Master Dissertation

<ul class="publication">
    {% for item in site.data.publications %}
    {% if item.class == "mdissertation" %}
    <li> {{ item.authors }} ({{ item.year }})
        <a href="{{ item.doi }}">{{ item.title }}</a>.
        <i>{{ item.institution }}</i>, {{ item.address }}.
    </li>
    {% endif %}
    {% endfor %}
</ul> 

## Bachelors Dissertation

<ul class="publication">
    {% for item in site.data.publications %}
    {% if item.class == "bdissertation" %}
    <li> {{ item.authors }} ({{ item.year }})
        <a href="{{ item.doi }}">{{ item.title }}</a>.
        <i>{{ item.institution }}</i>, {{ item.address }}.
    </li>
    {% endif %}
    {% endfor %}
</ul>