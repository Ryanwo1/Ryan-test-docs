---
layout: default
title: Navigation and View Tab
nav_order: 2
---

# Navigation and View Tab
{: .no_toc }

{: .fs-4 .fw-200 }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---


## Navigation introduction

```yaml
This page will give a gentle introduction to navigating Excel - namely the splash page and home page.
```

## Splash page


 When you launch Excel, you are met with the following page: <IMG HERE>
    
The top bar allows you to quickly create a new document. The first option on the left will create a new blank spreadsheet, and the options to the right are a basic Excel introduction (recommended for absolute beginners) and tutorials for various Excel features. Clicking on More templates will provide you with various skeleton files - handy when you want to quickly launch many kinds of charts and graphs.
    
Below the top bar you will find the search bar. The search bar is useful for finding a specific document when the name is known. 
    
Below the search bar are 3 options to find files when the name is not known. The first is Recent. Recent shows you your mostly recently used files, in descending order. Clicking on More workbooks will allow you to go back even further in time.
    
Pinned allows you to access files that you have pinned. Pinning a file marks it as one of your favourites and allows you to quickly access it next time. Pinning is a great option when you won't use a file on a regular basis, but the file needs to be found quickly and easily when it is needed. 
    
To pin a file, find it (either through the Search bar or through the Recent tab), right click it, then click on "Pin to list" <IMG HERE>. Your file will now immediately appear under the Pinned tab.
    
Shared with Me will show you documents that have been specifically shared with you. This allows you to more easily sort out documents that are part of a team effort.
    

## Home

The Home tab is the default tab when you launch Excel. If you wish to return to it, simply look at the top left of the Splash page. Home the very first tab.


## New

The New tab is located on the upper-left side of the splash page, below the Home tab. The New tab is used when you wish to create a brand-new document. You are able to create more than just a blank document:  the New tab will provide you with several template options. Should you desire a template that isn't under the new tab, you can use the search bar to search for a more specialized template. Excel even provides suggested search terms to get you started.

## Open

Open is on the splash page, on the upper-left side. Open can be found directly under New. Open allows you to open a folder or workspace by finding it manually on your computer. 
Clicking on Browse will open up your Explorer, where you can navigate your Computer's file hierarchy and manually select the document you wish to open.

The Open tab even supports opening documents that are Cloud-based (stored on the internet, not physically on your machine)

## Info

```yaml
The info tab does much more than simply provide info and deserves an investigation!
```

The info tab's primary purpose is to provide information about the document, as the name suggests.

The right side of the Info tab will tell you when the document was created, who created it, and when the document was last changed.
It also tells you the size of the file and allows you to categorize your file.

**The info tab has its own important functionalities, however:**

- The Protect Workbook option will control who can make what changes on your file. If you do not use this feature, anyone who has access to viewing the document can make changes to it. Someone can (through accident or through malice) erase all your data and hard-work!
- Inspect Workbook looks over your shoulder and protects you from things you might have missed. For example, Inspect Workbook can tell you when your file will leak personal information, or if your Excel file will not be compatible with different versions of Excel.
- Version History is Excel's internal version of version control. If you make a change that you want to revert (wrong data or the file stopped working after a change) then Version History will help you go back to an earlier version. **Note that you must sign in for your change history to be logged**
- Manage Workbooks deals with current and very recent Excel files. It will allow you to recover or delete current unsaved workbooks. Note that unsaved files will not be accessable for very long before they are lost forever, if you need to keep a file then save it to guarantee you will be able to access it in the future.
- Browser view options                          - 



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

