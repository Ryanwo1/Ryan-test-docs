---
layout: default
title: Navigation and View Tab
nav_order: 2
---

# Navigation and View Tab
{: .no_toc }

Excel navigation...
{: .fs-6 .fw-300 }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---


View this site's [_config.yml](https://github.com/pmarsceill/just-the-docs/tree/master/_config.yml) file as an example.


## Navigation introduction

```yaml
This page will give a gentle introduction to navigating Excel - namely the splash page and home page.
```

## Splash page

```yaml
search:
    When you launch Excel, you are met with the following page: <IMG HERE>
    
    The top bar allows you to quickly create a new document. The first option on the left will create a new blank spreadsheet, and the options to the right are a basic Excel introduction (recommended for absolute beginners) and tutorials for various Excel features. Clicking on More templates will provide you with various skeleton files - handy when you want to quickly launch many kinds of charts and graphs.
    
    Below the top bar you will find the search bar. The search bar is useful for finding a specific document when the name is known. 
    
    Below the search bar are 3 options to find files when the name is not known. The first is Recent. Recent shows you your mostly recently used files, in descending order. Clicking on More workbooks will allow you to go back even further in time.
    
    Pinned allows you to access files that you have pinned. Pinning a file marks it as one of your favourites and allows you to quickly access it next time. Pinning is a great option when you won't use a file on a regular basis, but the file needs to be found quickly and easily when it is needed. 
    
    To pin a file, find it (either through the Search bar or through the Recent tab), right click it, then click on "Pin to list" <IMG HERE>. Your file will now immediately appear under the Pinned tab.
    
    Shared with Me will show you documents that have been specifically shared with you. This allows you to more easily sort out documents that are part of a team effort.
```

    When you launch Excel, you are met with the following page: <IMG HERE>
    
    The top bar allows you to quickly create a new document. The first option on the left will create a new blank spreadsheet, and the options to the right are a basic Excel introduction (recommended for absolute beginners) and tutorials for various Excel features. Clicking on More templates will provide you with various skeleton files - handy when you want to quickly launch many kinds of charts and graphs.
    
    Below the top bar you will find the search bar. The search bar is useful for finding a specific document when the name is known. 
    
    Below the search bar are 3 options to find files when the name is not known. The first is Recent. Recent shows you your mostly recently used files, in descending order. Clicking on More workbooks will allow you to go back even further in time.
    
    Pinned allows you to access files that you have pinned. Pinning a file marks it as one of your favourites and allows you to quickly access it next time. Pinning is a great option when you won't use a file on a regular basis, but the file needs to be found quickly and easily when it is needed. 
    
    To pin a file, find it (either through the Search bar or through the Recent tab), right click it, then click on "Pin to list" <IMG HERE>. Your file will now immediately appear under the Pinned tab.
    
    Shared with Me will show you documents that have been specifically shared with you. This allows you to more easily sort out documents that are part of a team effort.

## Home

```yaml


```

## Heading anchor links

```yaml
# Heading anchor links appear on hover over h1-h6 tags in page content
# allowing users to deep link to a particular heading on a page.
#
# Supports true (default) or false
heading_anchors: true
```

## Footer content

```yaml
# Footer content
# appears at the bottom of every page's main content
# Note: The footer_content option is deprecated and will be removed in a future major release. Please use `_includes/footer_custom.html` for more robust
markup / liquid-based content.
footer_content: "Copyright &copy; 2017-2020 Patrick Marsceill. Distributed by an <a href=\"https://github.com/pmarsceill/just-the-docs/tree/master/LICENSE.txt\">MIT license.</a>"

# Footer last edited timestamp
last_edit_timestamp: true # show or hide edit time - page must have `last_modified_date` defined in the frontmatter
last_edit_time_format: "%b %e %Y at %I:%M %p" # uses ruby's time format: https://ruby-doc.org/stdlib-2.7.0/libdoc/time/rdoc/Time.html

# Footer "Edit this page on GitHub" link text
gh_edit_link: true # show or hide edit this page link
gh_edit_link_text: "Edit this page on GitHub."
gh_edit_repository: "https://github.com/pmarsceill/just-the-docs" # the github URL for your repo
gh_edit_branch: "master" # the branch that your docs is served from
# gh_edit_source: docs # the source that your files originate from
gh_edit_view_mode: "tree" # "tree" or "edit" if you want the user to jump into the editor immediately
```

_note: `footer_content` is deprecated, but still supported. For a better experience we have moved this into an include called `_includes/footer_custom.html` which will allow for robust markup / liquid-based content._

- the "page last modified" data will only display if a page has a key called `last_modified_date`, formatted in some readable date format
- `last_edit_time_format` uses Ruby's DateTime formatter; see examples and more information [at this link.](https://apidock.com/ruby/DateTime/strftime)
- `gh_edit_repository` is the URL of the project's GitHub repository
- `gh_edit_branch` is the branch that the docs site is served from; defaults to `master`
- `gh_edit_source` is the source directory that your project files are stored in (should be the same as [site.source](https://jekyllrb.com/docs/configuration/options/))
- `gh_edit_view_mode` is `"tree"` by default, which brings the user to the github page; switch to `"edit"` to bring the user directly into editing mode

## Color scheme

```yaml
# Color scheme supports "light" (default) and "dark"
color_scheme: dark
```
<button class="btn js-toggle-dark-mode">Preview dark color scheme</button>

<script>
const toggleDarkMode = document.querySelector('.js-toggle-dark-mode');

jtd.addEvent(toggleDarkMode, 'click', function(){
  if (jtd.getTheme() === 'dark') {
    jtd.setTheme('light');
    toggleDarkMode.textContent = 'Preview dark color scheme';
  } else {
    jtd.setTheme('dark');
    toggleDarkMode.textContent = 'Return to the light side';
  }
});
</script>

See [Customization]({{ site.baseurl }}{% link docs/customization.md %}) for more information.

## Google Analytics

```yaml
# Google Analytics Tracking (optional)
# e.g, UA-1234567-89
ga_tracking: UA-5555555-55
ga_tracking_anonymize_ip: true # Use GDPR compliant Google Analytics settings (true by default)
```

## Document collections

By default, the navigation and search include normal [pages](https://jekyllrb.com/docs/pages/).
Instead, you can also use [Jekyll collections](https://jekyllrb.com/docs/collections/) which group documents semantically together.

For example, put all your documentation files in the `_docs` folder and create the `docs` collection:
```yaml
# Define Jekyll collections
collections:
  # Define a collection named "docs", its documents reside in the "_docs" directory
  docs:
    permalink: "/:collection/:path/"
    output: true

just_the_docs:
  # Define which collections are used in just-the-docs
  collections:
    # Reference the "docs" collection
    docs:
      # Give the collection a name
      name: Documentation
      # Exclude the collection from the navigation
      # Supports true or false (default)
      nav_exclude: false
      # Exclude the collection from the search
      # Supports true or false (default)
      search_exclude: false
```

You can reference multiple collections.
This creates categories in the navigation with the configured names.
```yaml
collections:
  docs:
    permalink: "/:collection/:path/"
    output: true
  tutorials:
    permalink: "/:collection/:path/"
    output: true

just_the_docs:
  collections:
    docs:
      name: Documentation
    tutorials:
      name: Tutorials
```

