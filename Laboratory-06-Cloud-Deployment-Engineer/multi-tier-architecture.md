# Multi-Tier Architecture

## What is a Two-Tier Architecture?

A two-tier architecture is a software design in which an application is divided into two main parts: the web/application tier and the database tier. These two tiers work together to provide services to users. In this laboratory activity, Nextcloud serves as the web application, while MariaDB serves as the database.

## The Web/Application Tier

The web/application tier is responsible for providing the user interface and handling HTTP requests from users. In this activity, Nextcloud is the web application that allows users to access and manage their files through a web browser. It communicates with the database to store and retrieve information.

## The Database Tier

The database tier is responsible for storing and managing persistent information, such as user accounts, configuration data, and file metadata. In this activity, MariaDB acts as the database for Nextcloud. It allows the application to retrieve and save the information it needs.

## Why Separate Them?

Separating the web application and database into two containers makes the system easier to manage and maintain. Each container can be updated, restarted, and configured independently without requiring both services to be placed in one container. This separation also makes it easier to scale and troubleshoot the application.

