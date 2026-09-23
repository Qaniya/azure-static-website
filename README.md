# Azure Static Website Deployment

A beginner-level **Microsoft Azure Fundamentals** project demonstrating how to host a static website using **Azure Storage Account Static Website hosting**.

This project focuses on understanding basic Azure services, cloud storage, static website hosting, and deploying web files to the cloud using the Azure Portal.

---

## Project Overview

In this project, I created a simple static website using **HTML5 and CSS3** and hosted it on **Microsoft Azure Storage**.

Instead of using a traditional web server or virtual machine, Azure Storage Static Website hosting was used to make the website publicly accessible through an Azure-provided endpoint.

The main purpose of this project was to gain practical, hands-on experience with **Azure Fundamentals**.

---

## Learning Objectives

Through this project, I aimed to understand:

* What an Azure Storage Account is
* How Azure Storage works
* How static website hosting works
* How to create and configure an Azure Storage Account
* How to enable Static Website hosting
* How to use the `$web` container
* How to upload website files to Azure Storage
* How Azure provides a public website endpoint
* Basic cloud deployment concepts

---

## Architecture

The project uses a simple Azure Storage architecture:

```text
                 ┌─────────────────┐
                 │      User       │
                 │    Browser      │
                 └────────┬────────┘
                          │
                          ▼
                 ┌─────────────────┐
                 │ Azure Storage   │
                 │    Account      │
                 └────────┬────────┘
                          │
                          ▼
                 ┌─────────────────┐
                 │ Static Website  │
                 │      $web       │
                 └────────┬────────┘
                          │
                 ┌────────┼────────┐
                 ▼        ▼        ▼
            index.html style.css 404.html
```

---

## Technologies & Azure Services

| Technology / Service  | Purpose                             |
| --------------------- | ----------------------------------- |
| HTML5                 | Website structure                   |
| CSS3                  | Website styling                     |
| Microsoft Azure       | Cloud platform                      |
| Azure Storage Account | Stores and hosts website files      |
| Azure Static Website  | Hosts the static website            |
| Azure Portal          | Creates and manages Azure resources |

---

# Implementation

## Step 1 — Create an Azure Storage Account

I created an **Azure Storage Account** using the Azure Portal.

The Storage Account provides the cloud storage required for the website.

---

## Step 2 — Enable Static Website

I enabled the **Static Website** feature in the Storage Account.

The following settings were configured:

* **Index document:** `index.html`
* **Error document:** `404.html`

Azure automatically provides a special container called:

```text
$web
```

This container is used to store the files required for the static website.

---

## Step 3 — Create Website Files

I created a simple website using HTML and CSS.

### Project Structure

```text
azure-static-website/
│
├── index.html
├── style.css
├── 404.html
└── README.md
```

---

## Step 4 — Upload Files to Azure

The website files were uploaded to the Azure Storage `$web` container.

```text
$web/
│
├── index.html
├── style.css
└── 404.html
```

---

## Step 5 — Access the Website

After uploading the required files, I accessed the website using the **Primary Web Endpoint** provided by Azure Storage.

The website was successfully hosted and made accessible through the Azure endpoint.

---

#  Screenshots

## Azure Storage Account

Storage Account created for the project.

---

## Static Website Configuration

Static Website hosting enabled in the Azure Storage Account.

---

## Static Website Endpoint

Azure Static Website configuration and endpoint.

---

## Website Files

Website files uploaded to the `$web` container.

---

## Live Website

The final website running through the Azure Static Website endpoint.

---

# Challenge Faced

Initially, the website was not accessible because the Static Website configuration was not correctly configured.

I checked the Storage Account settings and verified that:

* Static Website hosting was enabled
* `index.html` was configured correctly
* `404.html` was configured correctly
* Website files were uploaded to the `$web` container

After correcting the configuration, the website became accessible through the Azure endpoint.

---

# What I Learned

This project helped me gain practical knowledge of fundamental Azure concepts, including:

* Azure Storage Accounts
* Azure Storage containers
* Static Website hosting
* `$web` container
* Azure Portal
* Cloud-based website hosting
* Azure resource configuration
* Basic cloud deployment

---

# Future Improvements

As I continue learning Azure, I can extend this project by exploring:

* Custom Domain configuration
* HTTPS
* Azure CDN / Azure Front Door
* Azure CLI
* Azure monitoring
* Additional Azure Storage features


