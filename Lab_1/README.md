# Lab 1

## Overview

Migrate a Canvas App and a Flow from one environment to another.

## Prequisites

Downloaded repository to local file system.

## Steps

### 1. Import Package to Development Environment

Open [Power Apps Studio](https://make.powerapps.com/).

Select your **Development** environment.

Click **Apps**.

Click **Import canvas app**.

Click **Upload**.

Navigate to the **Lab 1** folder in the repository folder.

Select the package `Package.zip`.

Click **Open**.

In the **Review Package Content** area:

* On the **Migrate - Lab 1 - Canvas App** row click **Update**, set **Setup** to `Create as new` and click **Save**.
* On the **Migrate - Lab 1 - Flow 1** row click **Update**, set **Setup** to `Create as new` and click **Save**.

Click **Import**.

Note: It might take several minutes for the components to import and show up in **Apps** and **Flows**.

Click **Flows**.

Click the **Ellipsis Icon** next to the **Migrate - Lab 1 - Flow 1** flow.

Click **Turn On**.

## 2. Run the App

Click to **Apps**.

Click the **Ellipsis Icon** next to the **Migrate - Lab 1 - Canvas App** app.

Click **Play**.

When the app opens, click **Submit**.

If **Name** is `Malcolm Reynolds`, then output would be `Hi, Malcolm Reynolds!`.

## 3. Create a Solution

Click **Solutions**.

Click **New Solution**.

* Set **Display name** to `Migrate - Lab 1 Solution`.
* Set **Publisher** to an existing publisher or click **New publisher** to create a publisher.

Click **Create**.

Click **Add existing**, then **App** and then **Canvas app**.

Click the **Outside Dataverse** tab.

Select **Migrate - Lab 1 - Canvas App** and click **Add**.

Click **Add existing**, then **Automation** and then **Cloud flows**.

Click the **Outside Dataverse** tab.

Select **Migrate - Lab 1 - Flow 1** and click **Add**.

## 4. Update Connectors in the Canvas App

We now need to update the Canvas App to use the flow that is part of the solution.

Still in the solution, click the **Ellipsis Icon** next to the **Migrate - Lab 1 - Canvas App** app.

Click **Edit**.

The app will open in the editor.

Click the **Power Automate** tab.

Select the **Ellipsis Icon** next to the **Migrate - Lab 1 - Flow** flow.

Click **Remove from app**.

Click **Add flow**.

Select the **Migrate - Lab 1 - Flow** flow.

Click **Save**.

Click **Publish**.

Click **Publish this version**.

Click **Back** in the toolbar.

Click **Leave**.

It should bring you back to the solution, then click **Publish all customizations**.

Click **Publish all customizations**.

## 5. Export the Solution in Development Environment

Click **Overview**.

Click **Export**.

On the **Before your export** panel, click **Next**.

Click **Export**.

From the notification bar, click **Download**.

## 6. Import Solution to Test Environment

Select your **Test** environment.

Click **Solutions**.

Click **Import solution**.

On the **Import a solution** panel, click **Browse**.

Select the exported package, e.g., `MigrateLab1Solution_1_0_0_1_managed.zip`.

Click **Next**.

Click **Import**.

Note: It might take several minutes for the components to import and show up in **Apps** and **Flows**.

Repeat the **Run the App** step.
