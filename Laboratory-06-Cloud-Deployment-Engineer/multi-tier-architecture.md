# Multi-Tier Architecture

## What Is a Two-Tier Architecture?

A two-tier architecture is a system that separates an application into two main parts: the web/application tier and the database tier. These tiers communicate with each other to provide services to users.

## The Web/Application Tier

The web/application tier handles user requests and displays the application's interface. In this mission, Nextcloud runs in this tier and allows users to access the private cloud storage system through a web browser.

## The Database Tier

The database tier stores and manages persistent information required by the application. In this deployment, MariaDB stores Nextcloud's database information, such as user accounts and file metadata.

## Why Separate Them?

Separating the web application and database into different containers makes the system easier to manage, maintain, and troubleshoot. Each service can be configured or updated independently, and separating their responsibilities helps organize the application. Docker Compose connects the containers so they can communicate with each other.
