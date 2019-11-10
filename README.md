# RT2 Lab Website

This website is built with [Jekyll](https://jekyllrb.com/).

## Setup

``` bash
brew install ruby
gem install bundler jekyll
```

Clone this repository, then install the dependencies:

``` bash
bundle install
```

## Run

Run the local webserver with:

``` bash
bundle exec jekyll serve
```

## Contribute

### Add a new member

New members are stored as markdown files under [_pages/team/_posts](_pages/team/_posts).

Each new member `.md` file must look like this:

``` yaml
---
layout: member
category: staff
title: Name of the member
image: Image filename, stored in /images
role: Member role
permalink: 'team/member-slug'
social:
    twitter: https://twitter.com/member
    linkedin: https://linkedin.com/in/member
    google-scholar: https://scholar.google.com/citations?user=member-id
education:
 - Education 1
 - Education 2
---

Write her bio text.
```

### Add a new publication

Publications are stored as `.yml` file under [_data/publist.yml](_data/publist.yml).

Just add a new entry to the list like this:

``` yaml
- title: "Celecoxib With Neoadjuvant Chemotherapy for
          Breast Cancer Might Worsen Outcomes
          Differentially by COX-2 Expression and ER Status:
          Exploratory Analysis of the REMAGUS02 Trial"
  image:
  description:
  authors: Hamy et al.
  year: 2019
  journal: Journal of Clinical Oncology
  link:
    url: https://www.ncbi.nlm.nih.gov/pubmed/30702971
    display: Pubmed Link
```

### Add news

Publications are stored as `.yml` file under [_data/news.yml](_data/news.yml).

An entry looks like the following:

```yaml
- date: 03/09/19
  title: "Something great"
  tags:
    - some
    - tags
  content: Lorem ipsum dolor sit amet, consectetur adipiscing elit,
    sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
    Eu turpis egestas pretium aenean. Luctus venenatis lectus magna fringilla
    urna porttitor. Lorem ipsum dolor sit amet. Pellentesque massa placerat
    duis ultricies. Commodo viverra maecenas accumsan lacus vel.
```

### Edit template

We use [Bootstrap](https://getbootstrap.com/) for designing the website. Feel free to modify either the [_pages](_pages/) or the
[_layouts](_layouts/) components.
