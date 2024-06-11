# Project: Deploying a LEMP Stack Website on AWS Cloud

## Overview
In this project, I will deploy a LEMP (Linux, Nginx, MySQL, PHP) stack website on the AWS (Amazon Web Services) Cloud. This project consists of six main steps:

0. **Step 0 — Preparing prerequisites**
   - In order to complete this project you will need an AWS account and a virtual server with Ubuntu Server OS.
   - If you do not have an AWS account, sign in to AWS free tier account and create a new EC2 Instance of t2.nano family with Ubuntu Server 22.04 LTS (HVM) image. Remember, you can have multiple EC2 instances, but make sure you STOP the ones you are not working with at the moment to save available free hours.

1. **Step 1 —  Installing Nginx and Updating the Firewall**
   - Install Nginx, a high-performance web server.
   - Update firewall settings to allow traffic on port 80.

2. **Step 2 — Installing MySQL**
   - Install MySQL, a popular relational database management system.
   - Secure the MySQL installation by running a security script.

3. **Step 3 — Installing PHP**
   - Install PHP and necessary modules to enable Nginx to handle PHP files.

4. **Step 4 — Configuring Nginx to Use PHP Processor**
   - Configure Apache to serve your website files from a custom directory.
   - Create a server block configuration file for your website.

5. **Step 5 — Testing PHP with Nginx**
   - Create a PHP script to test PHP processing and display server information.

6. **Step 6 — Testing PHP with Nginx**
   - Create a test database and configure access to it.
   - Write a PHP script to query data from the database and display it.
