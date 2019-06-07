---
title: [Set entity categories for SearchIQ ]
keywords: tbd
last_updated: tbd
summary: "You can specify a per column entity category to help SearchIQ."
sidebar: mydoc_sidebar
permalink: /:collection/:path.html
---

[SearchIQ]({{ site.baseurl}}/end-user/search/about-searchiq.html) is a search
experience that allows you to ask more natural questions, similar to the way you
might talk to a person.

If you have access to tables and worksheets for data modeling purposes, you can
specify entity types for their columns. This lets you designate that column as representing a person, place, or thing. So then when a user asks "Which", "Who", or "Where", an appropriate response can more easily be found in the data.

If you're not sure how to change the data modeling settings, see the
[Overview of data modeling settings]({{ site.baseurl}}/admin/data-modeling/data-modeling-settings.html).

## About Entity Categories

These are the available Entity Categories:

| Category            | Description                                          |
| :---                | :---                                                 |
| PERSON              | Contains data that represents a person, relevant to questions about "who?" |
| PLACE               | Contains data that represents a location, relevant to questions about "where?" |
| TIME                | Contains data that represents a date or time, relevant to questions about "when?" |
| PRODUCT             | Contains data that represents a product|
| ZIP_CODE            | Contains zip code data, relevant to questions like "where?" or "what zip code?"|
| LAT_LONG            | Contains data that represents geographical positioning, relevant to questions like "where?"|
| COMPANY_ORG         | Contains data that represents a company or organization |
| NUM_TYPES           | Contains numerical data |

## Set Entity Categories

To specify entity categories:

1. Click **Data** in the top menu, and choose **Tables** or **Worksheets**.

2. Click the name of your table or worksheet.

3. On the **Columns** tab, find the COLUMN NAMES for which you want to specify entity categories, and scroll to the right to find `ENTITY CATEGORY`.

4. Use the drop-down menu to set the `ENTITY CATEGORY` to the type you want.

5. Click **SAVE CHANGES** in the upper right.


## Related information

* [SearchIQ]({{ site.baseurl}}/end-user/search/about-searchiq.html)

* [Overview of data modeling settings]({{ site.baseurl}}/admin/data-modeling/data-modeling-settings.html)