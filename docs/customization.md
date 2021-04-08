---
layout: default
title: Data Analysis
nav_order: 6
---

# Data Analysis
{: .no_toc }


## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---
Microsoft Excel has become one of the most widely used software in all the industries. And data analysis is one of the most important functionalities in Excel which includes sorting, conditional formatting, charts and so on.

## Sorting

### Sort Sheet or sort range

Sort sheet means when we sort a category of values according to a specific pattern, all other correlated values will be moved because of it. Let’s read the example below.

In the original worksheet, all the information was sorted by the “Homeroom” column. However, if we sort the whole sheet again alphabetically by the “Last Name” of people, then not only the order of “Last Name” did change, but information in other columns which is related to this name also moves. 
Sort range means we only sort a part of the cells in a sheet, and it will be convenient when there are a few different tables in the same worksheet. Let’s read another example below. 


There are more than 1 table in the sheet, so we only want to sort the “Total Orders (by Grade)” on the right. Then after sorting range alphabetically by “Class”, all the cells of “Payment Method” on the left will never be affected. 

### Insturcions
1.Sort Sheet

Goal: Sort the whole sheet alphabetically by “Last Name”.
Select any cells in the “Last Name” column. For instance, we choose C2 this time. 

Find “Data” on the top of the menu, and click the “A-Z” command to rank names from initial A to initial Z.  
The result has been presented below. 


## Custom schemes

### Define a custom scheme

You can add custom schemes.
If you want to add a scheme named `foo` (can be any name) just add a file `_sass/color_schemes/foo.scss` (replace `foo` by your scheme name) 
where you override theme variables to change colors, fonts, spacing, etc.

Available variables are listed in the [_variables.scss](https://github.com/pmarsceill/just-the-docs/tree/master/_sass/support/_variables.scss) file.

For example, to change the link color from the purple default to blue, include the following inside your scheme file:

#### Example
{: .no_toc }

```scss
$link-color: $blue-000;
```

_Note:_ Editing the variables directly in `_sass/support/variables.scss` is not recommended and can cause other dependencies to fail.
Please use scheme files.

### Use a custom scheme

To use the custom color scheme, only set the `color_scheme` parameter in your site's `_config.yml` file:
```yaml
color_scheme: foo
```

### Switchable custom scheme

If you want to be able to change the scheme dynamically, for example via javascript, just add a file `assets/css/just-the-docs-foo.scss` (replace `foo` by your scheme name)
with the following content:`

{% raw %}
    ---
    ---
    {% include css/just-the-docs.scss.liquid color_scheme="foo" %}
{% endraw %}

This allows you to switch the scheme via the following javascript.

```js
jtd.setTheme('foo');
```

## Override and completely custom styles

For styles that aren't defined as variables, you may want to modify specific CSS classes.
Additionally, you may want to add completely custom CSS specific to your content.
To do this, put your styles in the file `_sass/custom/custom.scss`.
This will allow for all overrides to be kept in a single file, and for any upstream changes to still be applied.

For example, if you'd like to add your own styles for printing a page, you could add the following styles.

#### Example
{: .no_toc }

```scss
// Print-only styles.
@media print {
  .side-bar, .page-header { display: none; }
  .main-content { max-width: auto; margin: 1em;}
}
```
