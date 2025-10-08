---
# Featured tags need to have either the `list` or `grid` layout (PRO only).
layout: list

# The title of the tag's page.
title: Portfolio

# The name of the tag, used in a post's front matter (e.g. tags: [<slug>]).
slug: projects
#Gives the blog what post are related to it. It needs a post with the same category

order: 2 #Hydejack uses this to sort featured pages (those in _featured_categories/) in its navigation bar or sidebar. Lower numbers appear first (e.g., order: 1 might be “Blog,” order: 2 your “Portfolio”).If you omit it, order will follow file creation order — but setting it explicitly ensures control.


image: /assets/img/blog/H101.png #This image acts as a preview thumbnail for the category (the portfolio section itself). Hydejack uses it when it lists featured categories or in previews (for example, on the homepage). It’s not mandatory, but highly recommended for consistent visuals.

#URl en la que se genera este archivo https://tusitio.com/portfolio/
permalink: /portfolio/


# (Optional) Write a short (~150 characters) description of this featured tag.
description: >
  These are my personal projects. All of shown projects are related to my participation

paginate: false #Normally, Jekyll can paginate a list of posts (page 1, page 2, etc.). But since your portfolio gallery already displays all items in one grid, we disable pagination. If you later have 50 + projects and want paging, you could set paginate: true and tweak the gallery to respect pagination.

show_title: true #Hydejack can optionally hide the big page header (false) or show it (true). We keep it true so visitors see “Portfolio” as a title above your gallery.

feature: true #This flag tells Hydejack that this page should appear as a featured category, so it shows up in navigation menus, the homepage, or sidebar highlights automatically. Your existing _featured_categories/example.md works exactly this way.


# (Optional) You can disable grouping posts by date.
# no_groups: true

# Exclude this example category from the sitemap.
# DON'T USE THIS SETTING IN YOUR CATEGORIES!
sitemap: false
---

# My personal & professional projects

{% include gallery.html collection=site.categories.projects %}


<!-- This is Liquid syntax (Jekyll’s templating language).
It inserts the contents of _includes/gallery.html into this page and passes in a variable:
collection=site.projects → “Use the projects collection (your posts in /projects/_posts/).”

So inside gallery.html, include.collection equals site.projects.
That’s how the gallery knows which posts to read. -->