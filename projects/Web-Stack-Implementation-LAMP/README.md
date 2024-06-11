# Project: Deploying a LAMP Stack Website on AWS Cloud

## Overview
In this project, I will deploy a LAMP (Linux, Apache, MySQL, PHP) stack website on the AWS (Amazon Web Services) Cloud. This project consists of five main steps:

0. **Step 0 — Preparing prerequisites**
   - In order to complete this project you will need an AWS account and a virtual server with Ubuntu Server OS.
   - If you do not have an AWS account, sign in to AWS free tier account and create a new EC2 Instance of t2.nano family with Ubuntu Server 22.04 LTS (HVM) image. Remember, you can have multiple EC2 instances, but make sure you STOP the ones you are not working with at the moment to save available free hours.

1. **Step 1 — Installing Apache and Updating the Firewall**
   - Install Apache HTTP Server, the most widely used web server software.
   - Update the firewall settings to allow traffic on port 80.

2. **Step 2 — Installing MySQL**
   - Install MySQL, a popular relational database management system.
   - Secure the MySQL installation by running a security script.

3. **Step 3 — Installing PHP**
   - Install PHP and necessary modules to enable Apache to handle PHP files.

4. **Step 4 — Creating a Virtual Host for Your Website Using Apache**
   - Configure Apache to serve your website files from a custom directory.
   - Create a virtual host configuration file for your website.

5. **Step 5 — Enabling PHP on the Website**
   - Configure Apache to prioritize PHP files over HTML files.
   - Test PHP installation by creating a PHP test script.

Let's dive into each step in detail.

---

## Step 1 — Installing Apache and Updating the Firewall

Apache HTTP Server is installed using Ubuntu's package manager 'apt'. After installation, the firewall settings are updated to allow traffic on port 80, the default port for web traffic.

---

## Step 2 — Installing MySQL

MySQL, a popular relational database management system, is installed using the 'apt' package manager. The MySQL installation is secured by running a security script to remove insecure default settings and lock down access to the database system.

---

## Step 3 — Installing PHP

PHP and necessary modules are installed using 'apt'. This step enables Apache to handle PHP files, allowing the server to process dynamic content for the website.

---

## Step 4 — Creating a Virtual Host for Your Website Using Apache

A virtual host configuration is created for the website to serve files from a custom directory. This step involves configuring Apache to recognize the new virtual host, enabling it to serve web pages from the specified directory.

---

## Step 5 — Enabling PHP on the Website

Apache's DirectoryIndex settings are modified to prioritize PHP files over HTML files. A PHP test script is created to verify the PHP installation and configuration. After testing, the PHP script is removed for security purposes.

---

Congratulations! You have successfully deployed a LAMP stack website on the AWS Cloud by following these five steps. You now have a functional web server with Apache, a database with MySQL, and PHP for dynamic content generation.

