---
title: [Migrate or restore Worksheets]
last_updated: 10/28/2019
summary: "You can export an entire ThoughtSpot worksheet in a flat-file format. After optional modification, you can migrate it to a different cluster, or restore it to the same cluster."
sidebar: mydoc_sidebar
permalink: /:collection/:path.html
---

In ThoughtSpot, you can download Worksheets to a flat file in `yaml` format, modify the file, and subsequently upload this file either to the same cluster, or to a different cluster. This mechanism supports several scenarios that you may encounter:

- <strong>Migrating from a development environment to a production environment</strong> by downloading the file from the development cluster and uploading the same file into the production cluster
- <strong>Implementing metadata changes outside ThoughtSpot UI</strong>, such as replacing the underlying tables for the entire table, or replacing a single column from one table with a column in another table
- <strong>Making bulk changes</strong>, such as mass renaming of objects defined by the worksheets, and managing duplicates

## Prerequisites

You must have **Edit** permissions for the worksheet.

## Export Worksheet

To export a worksheet, follow these steps:

1. Click **Data** on the top navigation bar.

2. Click the name of the worksheet you want to edit.

3. Click the ellipses ![more options menu]({{ site.baseurl }}/images/icon-ellipses.png){: .inline} (more options) menu in the upper-right side of the screen.

4. From the menu, select **Export Worksheet**.

   Here, we are downloading the *Sales* worksheet.

   ![Export Worksheet]({{ site.baseurl }}/images/worksheet-export.png "Export Worksheet")

5. The worksheet downloads into your default directory.

   You can access the downloaded `*.yaml` file, named for your worksheet either through the file system manager, or by clicking on the name of the downloaded file in the left bottom corner of your Internet browser.

    ![Open downloaded worksheet file]({{ site.baseurl }}/images/worksheet-export-complete.png "Open downloaded worksheet file")

## Working with the Worksheet yaml file

You can change the yaml file that represents the Worksheet by editing its content. See [YAML Worksheet specification]({{ site.baseurl }}/admin/worksheets/yaml-worksheet.html) for the full syntax of the YAML file.

## Update a Worksheet

To update an existing worksheet, follow these steps:

1. Click **Data** on the top navigation bar.

2. Click the name of the worksheet you want to edit.

3. Click the ellipses ![more options menu]({{ site.baseurl }}/images/icon-ellipses.png){: .inline} (more options) menu in the upper-right side of the screen.

4. From the menu, select **Update Worksheet from file**.

   Here, we are uploading the edited *Sales* worksheet.

   ![Start Worksheet update from file]({{ site.baseurl }}/images/worksheet-update-from-file.png "Start Worksheet update from file")

5. In the upload interface, click **Browse your files**.

   ![Find the Worksheet YAML file]({{ site.baseurl }}/images/worksheet-update-browse.png "Find the Worksheet YAML file")

6. In your file system, find and select the YAML file.

7. In the **Update worksheet** interface, click **Upload**.

   ![Upload the Worksheet]({{ site.baseurl }}/images/worksheet-update-upload.png "Upload the Worksheet")

8. If you constructed the Worksheet file correctly, the **Upload Worksheet** interface displays an *Upload successfull* message.

9. To examine the updated Worksheet, click **Go to Worksheet**.

   ![Go to updated Worksheet]({{ site.baseurl }}/images/worksheet-update-success.png "Go to updated Worksheet")

## Related Information
- [Worksheet YAML specification]({{ site.baseurl }}/admin/worksheets/yaml-worksheet.html)