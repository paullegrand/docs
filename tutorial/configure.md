# 2. Configure & Create Your Content

You now officially have a working local Craft CMS install!

In this section we’ll learn what to do with it:

1. Take quick tour of the control panel.
2. Configure and edit our blog content.
3. Build dynamic front end templates or work with the GraphQL API.

## Control panel tour

The control panel may seem a bit empty—that’s a feature, not bug! Craft doesn’t tell you how to structure your content, it provides a blank slate you can use to build with however you’d like.

Let’s take a quick tour of the control panel to get oriented.

TODO: screenshot default control panel (call out profile icon and edition+version?)

The place you landed is the Dashboard, which you can customize with various widgets. By default, we’ll see the Recent Entries we haven’t created yet, recent Craft News, a Support and Feedback options, and a notice about whether any software updates are available.

In the upper right corner you can choose the profile circle to edit your account details or log out.

In the opposite lower left corner, you’ll see your Craft edition (Solo) and current version number. If you’re the explore-ahead type, you can click that edition badge to switch to a trial of Craft Pro. It doesn’t expire and it won’t hurt anything, but that’s not what we’re doing right now.

To the left, then, is the sidebar navigation. (You may have to use the hamburger icon to expand the navigation if you’re working with a narrow-ish browser window.) Choose Utilities.

TODO: screenshot utilities

You probably won’t need to visit Utilies too often, but it has some helpful tools.

By default you’ll land on the System Report. These are key details about your Craft install, and while we’re here it’s a good idea to make sure that each of the items under “Requirements” has a green check mark next to it. If anything there does not have a green check mark, choose the “i” icon to see more information and see if it’s something you’re able to adjust and meet that requirement.

We won’t be using these utilities so you can skip ahead if you’d rather. But here’s a quick look at what they do:

- Updates will list software updates that are available for Craft CMS and any installed plugins.
- PHP Info lists exhaustive details about your environment’s PHP configuration that can be useful for troubleshooting.
- The Queue Manager lets you peek under the hood of the system Craft uses to run batches of small jobs. Things will show up and disappear themselves as jobs are queued up and completed.
- Clear Caches lets you select and clear types of temporary stored data Craft uses to stay fast.
- Deprecation Warnings will detail any outdated code you might be using, where to find it, and usually what to replace it with.
- Database Backup lets you easily make and optionally download a copy of your database.
- Find and Replace is a powerful tool you can use to find and replace text in your database.
- Migrations will list and run PHP instructions you write for programmatically changing stuff.

## Plugin Store

## Content in Craft CMS

The process of deciding what shape your content should take is referred to as “content modeling.” Once you’re familiar with Craft’s building blocks, it can be liberating and even fun to decide how you’ll use them to bring your project to life.

### Get familiar with content modeling in Craft

Let’s take a quick look at the key building blocks and then use them to set up our blog.

#### Sections

Sections are often where most of your content will live. A section is a collection of similar types of content, like a blog post, press release, or job listing. Each section is meant to have many Entries that each follow a specific URL pattern and use whatever set of custom input fields you decide it should have.

A job listing section, for example, might have fields for requirements, location and salary range. A blog post probably won’t need any of those, but certainly a post body, imagery, and categories or tags.


TODO: overview of demo Sections, Entries, Field Layouts and Fields (include Globals?) **key point: flexibility**

### Create blog fields

### Create a blog section

### Configure Globals

### Edit entries

TODO: edit blog entries
