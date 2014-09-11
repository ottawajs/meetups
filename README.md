# Ottawa.js Meetups

This is the repository for the slides presented at [Ottawa.js meetups](http://ottawajs.org).

To view the slides, go [here](http://ottawajs.org/meetups/).

- 2014
 - [September](2014/09-september)
 - [October](2014/10-october)
 - [November](2014/11-november)
 - [December](2014/12-december)

## Development

1) ``git clone`` this repository
2) If you don't have Node installed then [installed Node.js](https://github.com/joyent/node/wiki/installation).
3) Run ``npm install`` in the terminal from the cloned repo's directory
4) Run ``grunt serve`` to run local server on port 8000 - [http://localhost:8000]()


### Markdown

The slides are created using [reveal.js](https://github.com/hakimel/reveal.js) and use the [markdown plugin](https://github.com/hakimel/reveal.js#external-markdown).

You'll see that the ``index.html`` pages link to markdown files in the ``content/`` directories. These markdown files contain most of the content that makes up the slides.

The convention for separating markdown content into slides are as follows:

#### New Vertical Slide

By adding a newline followed by a ``--`` (2 hyphens) followed by a newline to the markdown doc, you get a new vertical slide:

```markdown

## Slide 1.1

--

## Slide 1.2

--

## Slide 1.3


```

#### New Horizontal Slide

By adding a newline followed by a ``---`` (3 hyphens) followed by a newline to the markdown doc, you get a new horizontal slide:

```markdown

## Slide 1

---

## Slide 2

--

## Slide 2.2


```



## Hosting

Once you've made changes to master, make sure to update the ``gh-pages`` branch of this repo so that GitHub hosts at [http://ottawajs.org/meetups]().

More information on GitHub pages can be found in the [GitHub guides](https://help.github.com/articles/creating-project-pages-manually).

### Example

```bash
git checkout gh-pages
git merge master
git push origin gh-pages
```