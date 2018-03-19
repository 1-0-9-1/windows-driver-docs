---
title: Add or Remove Drivers
description: Add or Remove Drivers
ms.assetid: d55c98d9-4536-4004-8bee-e95f665cb4ce
ms.author: windowsdriverdev
ms.date: 04/20/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# Add or Remove Drivers

> [!NOTE]
> This section is only for WLK submissions. For all other submissions, including submissions for Windows 10, use the [Windows Hardware Dev Center Dashboard](https://msdn.microsoft.com/windows/hardware/drivers/dashboard/index).

On the **Add or remove drivers** tab, you can start or stop distribution through Windows® Update for the drivers in a submission package.

**To find the submission package**

-   To find the submission package that you want to change, click one of the following column headings to sort the list of drivers:

    <table>
    <colgroup>
    <col width="50%" />
    <col width="50%" />
    </colgroup>
    <thead>
    <tr class="header">
    <th>Column heading</th>
    <th>Definition</th>
    </tr>
    </thead>
    <tbody>
    <tr class="odd">
    <td><p>Submission ID</p></td>
    <td><p>The ID associated with a submission. You can click a link to open the <strong>Submission ID Details</strong> page, and see the current distribution status or modify the distribution date. You can also enter the submission ID in the <strong>Go to Submission Details</strong> box, and then click <strong>Go</strong>.</p></td>
    </tr>
    <tr class="even">
    <td><p>Hardware ID</p></td>
    <td><p>The ID associated with a device.</p></td>
    </tr>
    <tr class="odd">
    <td><p>Category</p></td>
    <td><p>The driver type.</p></td>
    </tr>
    <tr class="even">
    <td><p>Driver Version</p></td>
    <td><p>The version of the driver to be distributed. You can click a link to download the driver package, and confirm that it is the package you want to distribute.</p></td>
    </tr>
    </tbody>
    </table>

     

By default, the list displays devices with submissions made in the last 30 days. To change the display, use the results filter. For more information about the results filter, see [Filter and Search Your Submissions](https://msdn.microsoft.com/library/windows/hardware/br230792.aspx).

To view all submissions made for a specific device, click the plus sign next to the submission ID for that device.

**Tip**  
To download the data in Microsoft® Excel format, click **Download data to Excel**.

 

## <span id="Changing_the_driver_distribution"></span><span id="changing_the_driver_distribution"></span><span id="CHANGING_THE_DRIVER_DISTRIBUTION"></span>Changing the driver distribution


After you select the submission you want to edit, under **Actions**, you can select either **Standard distribution** or **Advanced distribution (with targeting)** to specify the way that you want to distribute the submission.

Simple distribution allows you to add or remove a driver from your submission package. Advanced distribution also allows you to modify the way that a driver is available. For example, a driver may currently only be available to your test users, but you can specify that you want to distribute the driver to all users.

**To use standard distribution**

1.  In the submission form for the submission package you selected, under **Actions**, click **Standard distribution**.

2.  For each driver, select the system or systems for which you want the driver to be available, and then click **Submit**.

**To use advanced distribution**

1.  In the submission form for the submission package you selected, under **Actions**, click **Advanced distribution (with targeting)**.

2.  Select the drivers you want to manage, and then click **Next**.

3.  For the selected drivers, choose the public groups you want to be able to see the driver. These groups can be set by the original creator of the Hardware ID.

4.  For the selected drivers, choose your distribution setting. The options are:

    -   **Not Distributed**: Do not publish the driver to Windows Update.

    -   **Test**: Distribute to a select group for testing.

    -   **Distributed**: Publish the driver to Windows Update.

    -   **Original State**: The driver remains available to the group you originally selected, no matter what else changes on the page.

5.  To review the changes you have made, click **Next**. When the changes are correct, click **Finish**.

6.  On the submission ID form, in the Driver publication date section, enter the date after which you want the changes to appear on Windows Update, and then click **Finish**.

The day after your chosen publication date, the availability of your drivers will be changed on Windows Update.

## <span id="related_topics"></span>Related topics


[Devices Without Drivers](https://msdn.microsoft.com/library/windows/hardware/br230802.aspx)

[Driver Statistics](https://msdn.microsoft.com/library/windows/hardware/br230762.aspx)

[Filter and Search Your Submissions](https://msdn.microsoft.com/library/windows/hardware/br230792.aspx)

[Submit Revised Drivers to Windows Update](https://msdn.microsoft.com/library/windows/hardware/br230770.aspx)

 

 

