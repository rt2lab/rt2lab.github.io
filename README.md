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

### Edit Data

New data must be added under the [_data](_data/) directory:

- [news.yml](_data/news.yml): Add news
- [publist.yml](_data/publist.yml): Add publications
- [team_members.yml](_data/team_members.yml): Add new team members

Data from this directory can be used in pages as follows:

``` html
<ul class="list-unstyled">
    {% for article in site.data.news %}
        <li class="media">
            <div class="media-body">
            <h4 class="mt-0 mb-1">{{ article.title }}</h4>
            <p><small>{{ article.date }}</small></p>
            {{ article.content }}
            </div>
        </li>
    {% endfor %}
</ul>
```

### Edit template

We use [Bootstrap](https://getbootstrap.com/) for designing the website. Feel free to modify either the [_pages](_pages/) or the
[_layouts](_layouts/) components.
