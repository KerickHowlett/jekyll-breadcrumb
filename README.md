# jekyll-breadcrumb
---

This is a very easy to implement and modify Breadcrumb component that does not require any knowledge in Ruby or modifying your **\_config.yml** file.

How this works is that the breadcrumb partial template will take the URL of any given page where the partial is included, and will break the URI wherever there is a slash (/), while making the domain your "Home" link.

### Example
It will turn **http://yourdomain.com/archive/lorem-ipsum** into **Home / Archive / Lorem Ipsum**.

Now, for the current page that the breadcrumb partial is being implemented, it will take the *page.title* from your page's Front Matter. However, if it can't find one, the template will just simply use the URI.

The primary functionality of this is within the **breadcrumb.html** file.

The JavaScript file, **breadcrumb.js**, will help to make sure that no dashes, underscores, or any other URIEncodes will end up in your breadcrumbs.

The CSS file, **breadcrumb.css**, offers very minimal styling that is designed to help it be perfectly flushed beneath your page's header.

## Installation

1. Download this repo.
2. Put the **breadcrumb.html** file within your **\_includes** folder, along with all your other partials.
3. Put the **breadcrumb.js** and **breadcrumb.css** files into wherever you put such files within your project.
4. Make sure that you reference the JavaScript and CSS files within your `<head>` tags, or at least make sure to compile them with either GULP or GRUNT.
5. Lastly, make sure you insert `{% include breadcrumb.html %}` in whatever layout file you wish to have breadcrumbs.

## Contributions

If you wish to contribute to this package, then I'd be more than willing to checkout some of your contributions. Just follow the instructions below on how I would like for you to submit them, please.

1. Fork Repo
2. Create new branch off of **master** branch, and name it **feature/<feature-name>**.
3. Submit a Pull Request with a brief description on what your contribution is.
