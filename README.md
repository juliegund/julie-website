![license](https://img.shields.io/github/license/mashape/apistatus.svg)

This is the repo that runs [Julie Gunderson's website](https://www.juliegund.com)

## New blog posts

Here are the steps to follow to write a blog post on Julie's site

1. Install [Hugo](http://gohugo.io) - *NOTE: Please make sure it is at least version 0.55.6*
2. Clone this repo
3. If you want to fire up a local copy to see your changes as you go, enter this command in a terminal`hugo server -w --baseUrl="http://localhost:1313"`
4. You probably want to do the previous thing in another pane/window, as it needs to keep running. The -w watches for any changes and rebuilds on the fly. You have to reset the baseUrl or it will try to go to www.juliegund.com
5. If you want to make a new blog post, type in `hugo new blog/my-blog-name.md`

Blog post files are stored in `content/blog`

### Images in blog posts

If you want to have an image for the blog post, put it into the path at `static/images/blog` (for example, `/static/images/blog/my-cool-image.png). Add the following to the frontmatter of the blog post:

```
img: "images/blog/my-cool-image.png"
```

To have images embedded in a blog post, put them into `static/images/blog` as well, but where you want them in the post, use the following markdown:

```
![](/images/blog/my-embedded-image.png)
```

## About page

To edit the About page, edit the file at `content/about/_index.md`

## Other settings

There are a myriad of settings in the file `config.toml`.

## Background images

The front page background and the header background will cycle through whatever images are located in `static/img/header-slides-julie` directory.