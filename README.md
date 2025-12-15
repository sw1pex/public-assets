# Public Assets Repository

This repository contains public static assets used across multiple
projects. Assets are hosted on GitHub and delivered globally via
**jsDelivr CDN**.

The repository is intended to store images and other static files for: -
Email templates - Marketing campaigns - Websites and landing pages - UI
assets (icons, illustrations) - Branding materials

All files in this repository are publicly accessible and optimized for
fast delivery.

------------------------------------------------------------------------

## CDN Delivery

All assets are delivered via **jsDelivr** using the following URL
format:

https://cdn.jsdelivr.net/gh/`<owner>`{=html}/public-assets/`<path-to-file>`{=html}

### Example

https://cdn.jsdelivr.net/gh/your-org/public-assets/project-name/email/headers/welcome.png

------------------------------------------------------------------------

## Repository Structure

Assets are organized **by project first**, then by usage or category.

public-assets/
├── project-name/
│   ├── email/
│   │   ├── headers/
│   │   ├── footers/
│   │   └── banners/
│   ├── marketing/
│   │   ├── campaigns/
│   │   └── socials/
│   ├── branding/
│   │   ├── logos/
│   │   └── guidelines/
│   └── ui/
│       ├── icons/
│       └── illustrations/
├── another-project/
│   └── ...

------------------------------------------------------------------------

## Project Folder Naming

-   Use kebab-case
-   Short and descriptive
-   Examples:
    -   vohen-kebab
    -   daynow-jobs
    -   internal-website

------------------------------------------------------------------------

## File Naming Conventions

-   Use kebab-case
-   Use English names only
-   Avoid spaces and special characters
-   Include size or context if relevant

Examples: - welcome-header.png - promo-banner-1200x600.jpg -
logo-dark.svg - icon-check-24.svg

------------------------------------------------------------------------

## Updating Assets & Cache Busting

jsDelivr applies aggressive caching.

If an asset is updated but keeps the same filename, use a version query
parameter:

https://cdn.jsdelivr.net/gh/your-org/public-assets/project-name/email/banner.png?v=2

Recommended versioning: - ?v=2 - ?v=2025-01 - ?v=final

------------------------------------------------------------------------

## Usage in HTML / Email Templates

Always use absolute URLs.

Example:

`<img src="https://cdn.jsdelivr.net/gh/your-org/public-assets/project-name/email/headers/welcome.png" alt="Welcome banner" width="600" />`{=html}

------------------------------------------------------------------------

## Allowed Asset Types

-   Images: png, jpg, jpeg, webp, svg
-   Documents: pdf
-   Icons and UI assets

No executable files or scripts should be stored in this repository.

------------------------------------------------------------------------

## Access & Visibility

-   Repository visibility: Public
-   All assets are publicly accessible

Do not store: - Sensitive data - Private documents - Credentials or
secrets

------------------------------------------------------------------------

## When to Use This Repository

Use this repository when you need: - Stable CDN URLs - Fast global
delivery - Assets shared across environments - Simple asset management
without additional cloud setup

------------------------------------------------------------------------

## Maintainers

This repository is maintained by the internal team. All changes should
be reviewed before merging to main.

------------------------------------------------------------------------

## Notes

-   Do not rename files that are already in use
-   Removing assets may break existing emails or pages
-   Prefer adding new files instead of replacing existing ones
