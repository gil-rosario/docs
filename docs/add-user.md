---
sidebar_label: 'Add a User'
title: 'Add a User to a Workspace'
id: add-user
---

## Overview

As a Workspace Admin, you can add team members to your Astronomer Cloud Workspace. From here, you can grant them user roles with permissions for specific actions across the Workspace and the Deployments within it.

This guide provides steps for adding a user to an Astronomer Workspace.

## Prerequisites

To add a user to a Workspace, you must have:

- An [Organization on Astronomer Cloud](install-aws).
- Workspace Admin permissions.

## Step 1: Invite the User to Astronomer

If the user you want to add doesn't already have an account on Astronomer Cloud, tell them to go to https://cloud.astronomer.io and sign up. Once they create an account, they will see the following screen:

<div class="text--center">
  <img src="/img/docs/welcome-user.png" alt="Successful account creation screen" />
</div>

Make note of the user's account email for the next step.

## Step 2: Add the User

To add a user with an Astronomer Cloud account to your Workspace:

1. In the Astronomer UI, open your Workspace and go to the **Access** tab.
2. Click **Add member**:

    <div class="text--center">
      <img src="/img/docs/add-user.png" alt="Add member button in the access menu" />
    </div>

3. Enter the user's email from Step 1.
4. Set a Workspace role for the user. The available roles are:

    - **Workspace Viewer**: Has permission to view anything in the Workspace, including users, Deployments, and DAG code in the Airflow UI
    - **Workspace Editor**: Has Viewer permissions, plus permission to [deploy code](deploy-code) and [configure Deployments](configure-deployment)
    - **Workspace Admin**: Has Editor permissions, plus permission to add users, remove users, and assign user roles

5. Click **Add member**.

Once you add the user, their information will appear in the **Access** tab as a new entry in the **Members** table.