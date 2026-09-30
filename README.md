# Spirits of the Continent

Spirits of the Continent is a digital mythology catalogue and cultural archive focused on African deities, spirits, tricksters, monsters, and ancestral figures from across Sub-Saharan Africa. The project combines a landing page, curated mythology data, and an interactive catalog that lets users explore entries, filter them, and add their own contributions.

This project was built with vanilla HTML, CSS, and JavaScript to showcase a dataset-driven web application without frameworks.

## What the project does

The site has two main views:

- A landing page at index.html that introduces the project and presents the theme of a digital museum of African mythology.
- A catalogue page at hero.html where users can browse and interact with the collected mythology entries.

The JavaScript in scripts.js creates the catalogue experience by:

- storing the mythology data in a JavaScript array of objects
- rendering cards dynamically to the page
- filtering by type, region, country, tribe, and favorites
- searching by name, country, tribe, or description
- sorting entries alphabetically or by region/type
- allowing users to view full details in a modal
- enabling users to add, edit, and remove entries from the archive
- handling image uploads for custom entries

## Project overview

The project is centered around a dataset called mythsArray. Each item in the array represents a mythological figure and contains fields such as:

- id
- name
- type
- country
- region
- tribe
- description
- image
- lore

This structure allows each entry to behave like a reusable object within the app, making it easy to render, search, filter, and update.

## Features included

- Search bar for quick lookup by name or other metadata
- Type filters for Deity, Spirit, Trickster, Monster, and Ancestor
- Region filters for West Africa, East Africa, Central Africa, and Southern Africa
- Country and tribe dropdown filters
- Sort options for A–Z, Z–A, region, and type
- Favorite toggle to save and revisit selected entries
- Full detail modal showing extended lore and descriptive information
- Add-entry form for contributing new mythological figures
- Edit form for updating existing entries
- Remove function for deleting entries from the archive
- Responsive, museum-style visual design with a cinematic landing page

## File structure

- index.html — intro page / home screen for the project
- hero.html — main catalogue interface and interactive data browser
- style.css — the visual styling for both pages and catalogue components
- scripts.js — all dataset logic, DOM rendering, filters, modals, and interactivity
- assets/ — media and dataset imagery used by the site

## How the code works

The core behavior in scripts.js is driven by a filter state object called currentFilters, which tracks:

- the current search term
- active type filters
- active region filters
- selected tribe and country
- chosen sort order
- whether favorites-only mode is enabled

When the page loads, the app runs the following initialization flow:

1. renderMythsCatalogue() builds the visible cards
2. setupEventListeners() attaches all UI event handlers
3. populateTribeDropdown() and populateCountryDropdown() load available options
4. updateFavoritesCount() refreshes the favorites badge

The app then re-renders the catalogue whenever a user changes search, filters, sort order, or favorites.

## Running locally

To view the project locally:

1. Download or clone the repository.
2. Open index.html in a browser, or run a lightweight local server if preferred.
3. Navigate to the landing page and then enter the catalogue from there.

## Live site

https://wanjavwa.github.io/SnapChat-SEA-Project-Wanjavwa-Nzobokela/

## Summary

This repository is a complete mythology catalog website that preserves African storytelling traditions through an interactive, data-driven interface. It demonstrates front-end web development with data modeling, filtering, sorting, DOM manipulation, and user-generated content handling in a single-page JavaScript app.
