# Multi-Tier Architecture

## What is a Two-Tier Architecture?

An example of a two-tier architecture is the separation of a web application into a web/application tier and a database tier. The web/application tier provides a user interface and makes requests to the database tier to fulfill user requests. NextCloud is the web application in this lab and MariaDB is the database.

## The Web/Application Tier

The web/application tier is accountable for the interface and the management of user request. In this context, Nextcloud is a web application that provides users with access to their files via browsers. It interacts with the database for the storage and retrieval of data.

## The Database Tier

The tier of the database has an important role to play in keeping and managing many permanent data like user accounts, configuration details, file metadata, etc. MariaDB plays the part of the database in Nextcloud in this process. This way the application can store its information and use it when it is needed.

## Why Separate Them?

By putting the web app and database in the two containers the management and maintainability of the system becomes easier. Each container is able to be updated, restarted, and configured on its own. It helps to easily scale and fix issues within the application.

