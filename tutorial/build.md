# 3. Build Your Front End

## Choose your front end

Craft supports two different ways of building your front end:

1. Using Twig templates for server-generated pages.
2. Using a headless front end that gets its content from a GraphQL or JSON API.

If you’ve never built a website using either one, choosing is a matter of picking whatever you’re most comfortable with.

Twig templates are like plain HTML with superpowers. They live right in the Craft codebase you’ve already set up, and they’re easiest to start with if you want to start coding right now.

If you’re familiar with JavaScript and have built a site using Gatsby or Gridsome before, relying on Craft’s GraphQL API might be easier. You can spin up your front end project however you normally would, then configure Craft to make its content available.

TODO: compare working with Twig and GraphQL to someone who’s not done either, then link to template or GraphQL route

## Create templates

Craft ships with the ability to create a dynamic front end using Twig templates.

TODO: share set of demo files before we start, meant for copy+paste

TODO: explain markup, purpose of templates

TODO: mention other front end assets (but grab existing for tutorial)

TODO: create layout

TODO: create entry detail page (explain `_`)

TODO: create single template

TODO: create category index?

TODO: create category post listing (high-level routing overview)

### VS Code syntax highlighting

- Twig
- PHP
- JSON
- JavaScript?
- more useful plugins

## Fetch content with GraphQL

You can also use Craft CMS headlessly, meaning your web server provides an authoring experience but relies on outside code to provide the front end for visitors. In this case you won’t work with Twig templates, but Craft’s GraphQL API.

TODO: what is GraphQL

TODO: headless configuration

TODO: querying Entries, Globals, and Assets

TODO: sending data back to Craft (CSRF) ?

TODO: configuring Live Preview

## Install a plugin?
