# Log Jekyll Theme

A simple Jekyll Theme for keep a log of all your media consumption.

## _config.yml

In this file you can find the `author` and site `title`. The third element is the `description`. This element will be displayed as the second row of the black header in `index.html` and used a `meta-description`.

## Categories

Write all your media in `_data/log.yml` in the following categories:
- `data` per the time period.
- `book`. This is the only category that will accept multiple rows in the `log.yml` file.
- `music`
- `movie`
- `tvserie`
- `podcast`
- `youtube`
- `article`
- `manga`

### Add a category

You can add a category in the `log.yml` file and add the relative section in the `index.html`. Replace `[category]` with your new category without [].

Example of a section in `index.html`.

```html
{% if log.[category] %}
<div class="section">
  <span class="passive">&gt;_</span> Category
</div>
<ul>
  <li>{{ log.[category] }}</li>
</ul>
{% endif %}
```

## Highlight

A `<span class="title">` can be used for highlight a title.

## Favicon

You can use your favicon in the `<head>` of `index.html`.
