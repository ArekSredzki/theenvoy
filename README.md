# The Envoy Theme

A minimalistic theme for [Ghost](https://ghost.org/) designed for [The Envoy](http://theenvoy.ca/).

![The Envoy](assets/images/mockup.jpg)

## Installation

1. Download the theme from GitHub.
2. Upload the theme as described in the [Ghost Documentation](http://docs.ghost.org/usage/settings/).

Looking for more instructions? Sorry, it's just that easy.

## Enabling Disqus Comments

If you want to enable comments, simply open `post.hbs` and remove the exclamation mark in the comments block, so `{{!> comments}}` becomes `{{> comments}}`.

You'll also need to enter your Disqus "shortname". Just head on over to the [Disqus](http://disqus.com/) website and register for an account. They'll give you a small snippet of code, but all we need from it is the following line:

    var disqus_shortname = 'YOUR_SHORTNAME_HERE';

Once you have that, just open `partials/comments.hbs` and replace the `YOUR_SHORTNAME_HERE` variable with the one Disqus gave you. Try not to edit any other settings or replace the code though, it's preconfigured to work with Ghost.
