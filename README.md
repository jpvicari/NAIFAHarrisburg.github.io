# NAIFA
https://www.naifahbg.com

This is a [Jekyll](https://jekyllrb.com/) site hosted at [https://github.com/NAIFAHarrisburg/](https://github.com/NAIFAHarrisburg) by GitHub Pages.

## Getting started (To Run a Local Version of the Site)

1. Install Ruby v2 *(if not already installed)*
2. Clone repository
3. `cd` into repository
4. `gem install bundler`
5. `bundle install`
6. To run: `bundle exec jekyll serve` with optional `--incremental` flag

## Online Markdown Editor
This is a great online page/post editor for Markdown.
[Online Markdown Editor](https://dillinger.io/)

## Guides and rules for adding posts

All posts are added in markdown. Here's a [markdown cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) if you can't find it here.


### Featured Banner Post (pinning)

Add the tag `featured` to pin a post to the homepage masthead. This works on any `post`.

```
tag:
- featured
```
### linking

- external linking
```
[link text](https://external-link/here/ "any title text you want to include for increased SEO")
```

- `mailto` links
```
[contact us here](mailto:email@domain.com)
```

- posts using `post_url`. This tag places the domain structure for you when linking internally.
```
[link text]({% post_url name-of-post-with-dates %} "any title text you want to include for increased SEO" ).
```

### Images

#### Adding an image

Adding an image is easy enough, remember to add the Bootstrap 4 responsive image class `.img-fluid`.

```
![ Your image description, i.e., alt tag content ]( /path/to/image.jpg ){: .img-fluid }
```

#### JPG vs. PNG

All post, card and header images should be saved as `.jpg` using the specifications below.

|setting|default|
|---|---|
| dpi | 144* |
| max-width | 1200px |
| image quality | 80% |

> * 144dpi takes greater advantage of retina and 4K+ resolutions vs. the older 72dpi standard.

Logo images should always be saved as transparent `.png` files.

#### Naming convention

- **DO** use lowercase
- **DO** use hyphens
- **DO** use descriptive names for SEO

- **DO NOT** use spaces
- **DO NOT** use commas
- **DO NOT** use underscores
- **DO NOT** use CamelCase
- **DO NOT** use special characters (`!@#$%^*~`)
- **DO NOT** use the ampersand (`&`), spell out `and`

As we move forward, we'll also look at an image structure that will change based on screen size via `srcset` to deploy multiple sizes while targeting specific uses and screens.

### Tables

Markdown tabels are

```
header 1 |	header 2
--- | ---
column 1 | column 2
column 1 | column 2
column 1 | column 2
```
Adding Bootstrap classed directly before a table will add styling to your table. **Always use `.table`**, combine the rest for the desired effect.

class |	effect
--- | ---
table | Bootstrap default table styling
table-striped | alternating shaded backgrounds for better visibility
table-bordered | borders
table-inverse | dark table with white text

```
{: .table.table-striped.table-bordered.table-invert }
header 1 |	header 2
--- | ---
column 1 | column 2
```

### Typography

There are additional [classes dedicated to typography](http://v4-alpha.getbootstrap.com/content/typography/) that may help you achieve your desired effect.

> note: some classes may be overwritten by existing styles.
