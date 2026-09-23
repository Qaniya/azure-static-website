# 🚀 Azure Static Website Deployment

A beginner-level Azure Cloud project demonstrating how to deploy a static website using **Azure Storage Static Website hosting**.

This project was created as part of my hands-on Azure Cloud learning journey and portfolio development.

---

## 📌 Project Overview

In this project, I created a simple static website using HTML and CSS and deployed it using **Microsoft Azure Storage**.

Instead of using a traditional web server or virtual machine, the website is hosted using Azure Storage Static Website functionality.

### Technologies Used

- HTML5
- CSS3
- Microsoft Azure
- Azure Storage Account
- Azure Static Website
- Git
- GitHub

---

# 1. 🎯 Problem

Hosting a simple static website does not always require a traditional web server or virtual machine.

The objective of this project was to learn how to deploy HTML and CSS files to the cloud and make the website accessible through a public Azure endpoint.

---

# 2. 🏗️ Architecture

The basic architecture of this project is:

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
              ┌───────────┼───────────┐
              ▼           ▼           ▼
          index.html  style.css   404.html