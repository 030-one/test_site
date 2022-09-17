# WEBSITE TEMPLATE

A clean template for a personal blog or a different static website.

## Things to do

### Set a theme

Color theme can be declared in the `default.html`

Set a color theme in `_layouts/default.html`, on line 2 `class="NAME HERE"`.

To create a custom theme, add a new section in `_sass/_variables.scss`

Use this template to change things:

```scss
.<NAME HERE > {
  --body-color: <Text color>;
  --body-bg: <Background color>;
  --heading-color: <Heading color>;
  --link-color: <Link text color>;
  --link-hover-color: <Link text color on hover>;
  --border-color: <Color of horizontal lines and table borders>;
  --code-bg: <Background color of code blocks>;
  // more things can be added here, like font or other element colors
}
```

### Add icons

Add icons for your website in `assets`.

| Name                               | Type   | Size      | Usage                                                                        |
| ---------------------------------- | ------ | --------- | ---------------------------------------------------------------------------- |
| `apple-touch-icon-precomposed.png` | `.png` | 152 x 152 | icons that are used on apple devices when creating a shortcut                |
| `favicon.ico`                      | `.ico` | 50 x 50   | icon of the websitem visible in tab and when saved as bookmark or to desktop |

### Change general settings

Open `_config.yml` and change following settings

```text
title: <Title of your website>
url: <URL or domain of the website>

...

author:
  name: <Your name if you want to have it visible in posts>
  url: <Leave empty>
  email: <An email you want to be messaged under>

...

nav:
  - title: About
    url: /about
  - title <Name>
    url: <The link>

```

The `nav` part will be used when you want to have more items in the bar on the top right.

### Add Datenschutz

_It is recommended to have a text like this._

Add a text to `legal/datenschutz.md`.

A text can be generated here [https://www.e-recht24.de/](https://www.e-recht24.de/). There are also other generators. out there.

If you don't want a Datenschutztext, remove the line `<a href="/legal/datenschutz" title="Datenschutz">Datenschutz</a>` and the previous `|` in `_includes/footer.html` on line 6 and 7.

**I am not responsible for any legal damage you may experience when using this template**

### Change about page

Edit the contents of the `about.md` to include info about your website or your project.

### Add a contact page

Edit the contents of `contact.md` to include your contact info.

When doing this, add this to the `_config.yml' under the nav section as previously described.

```text
  - title Contact
    url: /contact
```

## Writing posts

Posts can be put in folders, these folders serve as a category, e.g. `Chatting/_posts/2021-01-12-A-Person-that-chats.md`

This would create a post called "A Person that chats" in the category "Chatting" written on the 12th of January 2021.

Every post has to start with

```text
---
layout: post
title: <TITLE HERE>
---
```

Then a blank line, and then the content of the post. The content needs to be written in [Markdown](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

## For more info

Do research, using the keywords `github pages` and/or `jekyll`.

## Using this template for GitHub pages

Create a new repository, choose this template when creating it, and give your repo a clear name.

Make the changes you want.

When you are ready,

1. go into your repository settings
1. on the left click on `Pages`
1. Under the `Source` section, click on the `None` field
1. Select `main`
1. Confirm using `save`

It will take a few minutes until the site is up.

You will get an email from GitHub if something should fail.
