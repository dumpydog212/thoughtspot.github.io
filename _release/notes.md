---
title: ["5.1 Release Notes"]
toc: false
keywords: "release notes"
last_updated: Jun 2019
sidebar: mydoc_sidebar
permalink: /:collection/:path.html
---

## What's in the Release Notes

ThoughtSpot version 5.1.4 is now available. These release notes include information about new features,
fixed issues from the previous releases, and any known issues.

* [5.1.4 Fixed Issues](#514-fixed)
* [5.1.3 Fixed Issues](#513-fixed)
* [5.1.2 Fixed Issues](#512-fixed)
* [5.1.1 New Features](#511-new)
* [5.1.1 Fixed Issues](#511-fixed)
* [5.1 New Features](#51-new)
* [5.1 Fixed Issues](#51-fixed)
* [Notes for older versions](#notes-for-older-versions)

## Supported Upgrade Paths

If you are running one of the following versions, you can upgrade to the 5.1.4 release
directly:

* 4.5.1.x to 5.1.4
* 5.1.x to 5.1.4

(This includes any hotfixes or customer patches on these branches.)

If you are running a different version, you must do a multiple pass upgrade.
First, upgrade to one of the above versions, and then to the 5.1.4 release.

{: id="514-fixed"}
## 5.1.4 Fixed Issues

An error that occurred when saving changes to the title of a visualization is now fixed.

Corrupted metadata after upgrade which made some worksheets uneditable is now fixed.

A problem with date filters in the Japanese locale is now fixed.

An issue with refreshing materialization of views is now fixed.

{: id="513-fixed"}
## 5.1.3 Fixed Issues

Downloading an R visualization no longer causes an empty page to be displayed.

A problem where tables in a Google Chrome tab become misaligned is now fixed.

Custom scatter charts no longer disappear from pinboards after an upgrade.

An issue where the Copy-and-edit button no longer appears on embedded visuals is now fixed.

Occasional slow navigation between the Answer and Pinboard pages has been fixed.

A normal bar chart in a pinboard which is changed to a stacked bar chart no longer reverts to the normal bar chart after the pinboard is saved, browser is closed, and pinboard is reopened.

A problem where using the exclude filter on pinboards causes the wrong results to be displayed is now fixed.

Usage-based indexing of search has been improved.

A problem where the `tscli ssl rm-cert` command was used to remove a cert, but did not revert it back to the default cert is now fixed.

When a search that uses no attributes results in fan-trap queries, the measure values shown are no longer incorrect.

A problem where some users could not log in through SSO after an upgrade has been fixed.

Fan-trap queries no longer have more grouping columns than necessary.

An issue with worksheets showing incomplete compound-column joins has been fixed.

A problem where the user interface becomes slow during a data load has been fixed.

CSVs downloaded by certain row-level-security users are no longer empty.

{: id="512-fixed"}
## 5.1.2 Fixed Issues

Search no longer stops working under certain conditions like fast typing, or copying and pasting of a search query.

Selecting 'Copy and Edit' in an answer, pinboard visualization, insight, SpotIQ pinboard or view, no longer causes the user to be signed out.

HDFS images for a cluster are now created prior to pushing the HDFS configuration. This ensures images are fresh during an upgrade.

When removing a node, the node calling command no longer results in unreachability due to misconfigured firewall settings.

Permissions issues with `tsload` and `tql` are now fixed, so the **thoughspot** user can load data.

Database stability has been improved.

{: id="511-new"}
## 5.1.1 New Features and Functionality

### Data visualization color refinements

Visualization colors have been refined to match ThoughtSpot's fresh, new look. You can still customize colors, and reset them to the default color palette later, if needed.

{: id="511-fixed"}
## 5.1.1 Fixed Issues

Geo Bubble map labels can now be disabled or enabled through a data labels checkbox.

Filter panel failure to open during formula creation has been fixed.

Custom R analysis failure when run from Custom Analyze has been fixed.

Microsoft Internet Explorer button display problem in Edit Group, Add a New Group, and Custom Analysis has been fixed.

Tooltips in line, scatter, and radar charts have been improved to avoid tooltip display when far from a data point.

Microsoft Internet Explorer problem with saving the name of an answer has been fixed.

Previously, admin style and font customizations for tables and charts were off by default. They are now on by default.

Search phrase autocomplete has been fixed to prevent unnecessary red highlighting of values.

Geo Bubble and Geo Heatmap issue where chart displays momentarily and then disappears has been fixed.

Zoom on Geo maps can now be done using a mouse scroll wheel.

{: id="51-new"}
## 5.1 New Features and Functionality

### Quick Select

When you type a phrase or a letter in the search bar, the first suggestion is
automatically highlighted and you can press Enter to select it ([Quick Select]({{ site.baseurl }}/end-user/search/about-the-search-bar.html)). Suggestions can be an attribute, measures, value, keyword, historical queries,
or exactly what you typed as the search phrase. Historic suggestions always
display on top with the first suggestion highlighted as default.  If there are
no suggestions, the suggestion list is not be displayed.

### Improvements in the presentation mode experience of pinboards

When you display pinboards charts on projectors in conference rooms and on a
laptop that has a widescreen display, the display automatically adjusts itself
depending on the size of the display screen. For example, if you are using a
widescreen display, pinboard font size increases for a more definitive and
high-quality experience.

1. Choose a pinboard that you want to display and click the **present** icon ![present icon]({{ site.baseurl }}/images/icon-present.png){: .inline} (top-right).

   Alternatively, you can click the ellipses ![more options menu icon]({{ site.baseurl }}/images/icon-ellipses.png){: .inline} and select **Present**.

2. Use the **Up** and **Down** arrow keys to navigate.

### Stable search suggestions

Search suggestions are now more stable. When you start to type a search phrase and
the full matching phrase appears in the results list, the order in which it
appears does not change as you finish typing it.

### Show rounded or non-rounded numbers on charts

You can set labels on charts to [show rounded or non-rounded numbers]({{ site.baseurl}}/end-user/search/show-data-labels.html#show-rounded-or-non-rounded-numbers).

### Pie charts now support color customization

You can now [customize the colors of each slice on pie charts]({{ site.based}}/end-user/search/change-chart-colors.html#set-pie-chart-slice-colors) from the chart Styles panel. Click the Styles button next to any pie chart to get started (![paintbrush icon]({{ site.baseurl }}/images/icon-paintbrush.png){: .inline}).

### Longer pinboard descriptions

Table or chart descriptions in a pinboard can now be up to two lines long.
Descriptions that exceed a second line are truncated with three periods (...) at
the end. Headline tiles (which don’t have a table or chart) are limited to a
one-line description.

### New typography in the desktop app

With the 5.1 release, the fonts used are Optimo Plain and BB Roller Mono. This
provides a modern, more readable look for the ThoughtSpot application user
interface and data visualizations.

### Table aggregate headline

The Table Aggregate headline option is available when an aggregate function is
used in a table either through a formula or a search bar query, like the average
of a measure. It recalculates the function for the entire table. In such cases,
the Table Aggregate is shown by default below the table, instead of the “Avg”
option, which does a second level of aggregation on top of the existing
aggregation.

### Period to date

Before 5.1, Period to Date didn't work in conjunction with other date filters.
With this release, you can compare data spread across the same period and drill
down to a specific period of a year, month, week, and date.

For example, you can compare:

* `quarter to date vs last year quarter to date`
* `month to date vs last month to date`
* `year to date vs last year month to date`
* `week to date vs last quarter week to date`

To review date keywords, see [Date in keywords reference]({{ site.baseurl }}/reference/keywords.html#date).

For more about `vs` keyword, see [Comparative in keywords reference]({{ site.baseurl }}/reference/keywords.html#comparative)

### Case sensitivity on formulas is supported

You can now enable case sensitivity when defining formulas, and the final
formula output retains the case sensitive state. Quoted text in a formula can
now be case-sensitive. For example, "`if revenue > 1000 then 'Good' else 'Bad'`".
The output of this formula retains the case.

### SpotIQ personalization

Users can specify "Insight Threshold Settings" as part of their individual
profile [SpotIQ preferences]({{ site.baseurl}}/end-user/introduction/about-user.html#spotiq-preferences-and-email-notifications) to further refine the parameters SpotIQ uses.
SpotIQ profile preferences are a subset of those available on the SpotIQ "Customize
analysis dialog", and persist for all SpotIQ analyses, unless you explicitly
reset options for custom analyze.

### Improved search editing

You can edit a search without affecting existing search results. You can insert a new phrase or edit an existing one in the middle of a search without causing any errors. You can even merge words or phrases without breaking the search. As you edit your search, ThoughtSpot continuously generates new results.

### Copy and edit

The previous feature called "Make a Copy" is now called "Copy and Edit" and it brings a major workflow improvement. Instead of simply saving a copy in the background, "Copy and Edit" allows you to make a copy of an answer, pinboard visualization, insight, SpotIQ pinboard or view and immediately start editing it.

### SpotIQ insight feedback

Administrators can save user feedback and use it to suppress down-voted insights
from auto or custom SpotIQ analyses.

### SpotIQ column level data modeling

Data modelers and administrators can [exclude columns from SpotIQ analyses]({{ site.baseurl }}/admin/data-modeling/spotiq-data-model-preferences.html) via a
new `SPOTIQ PREFERENCE` option on the Data tabs for worksheets, tables or views.
By default, all columns are included in SpotIQ analyses.

### Schema Viewer available to non-admin users

Starting in the 5.1 release, you can grant non-admin users with
[Can manage data]({{ site.baseurl}}/admin/users-groups/about-users-groups.html)
privilege access to [Schema Viewer]({{ site.baseurl}}/admin/loading/schema-viewer.html).
This enables non-admin users to view data in a schema they have access to.

### Active Directory (AD) management for ThoughtSpot nodes

ThoughtSpot supports enabling [Active Directory (AD) based access]({{ site.baseurl}}/admin/setup/active-directory-based-access.html) individually on
each node where the commands are run. To enable AD access on a cluster, the
administrator must run the same commands on each individual node and on any
additional nodes added to the cluster.

### Keyword support for eight new languages / locales (Beta)

Beta mode [internationalization (I18N) keywords support]({{ site.baseurl}}/reference/keywords.html) for the following additional locales is available in version 5.1:

* Español (España)
* Português (Portugal)
* Italiano
* Dansk
* Suomi
* Svenska
* Norsk
* Nederland

{: id="51-fixed"}
## 5.1 Fixed Issues

The X and Y axes were previously flipped on [bar charts and stacked bar charts]({{ site.baseurl }}/end-user/search/about-bar-charts.html). This has been fixed.


{: id="notes-for-older-versions"}
## Notes from older versions

* [5.0 Release Notes](/5.0/pdf/ThoughtSpot_Release_Notes_5.0.pdf)
* [4.5 Release Notes](/4.5/pdf/ThoughtSpot_Release_Notes_4.5.pdf)
* [4.4 Release Notes](/4.4/pdf/ThoughtSpot_Release_Notes_4.4.pdf)
* [4.2 Release Notes](/4.2/pdf/ThoughtSpot_Release_Notes_4.2.2.pdf)
* [3.5 Release Notes](/3.5/pdf/ThoughtSpot_Release_Notes_3.5.7.pdf)
