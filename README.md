# CQRS Warehouse Frontend

A small single-page web frontend for a warehouse demo application built on the CQRS (Command Query Responsibility Segregation) pattern. It talks to a separate backend service running locally. Commands go to the backend as POST requests, and queries read data back.

## Features

- Articles: list articles, create new ones and copy article identifiers
- Shipments: create shipments, unload incoming shipments into containers and send loaded shipments on their way
- Containers: see container details such as expiration date, reservation status and location, move containers and load reserved containers into trucks
- Customer requests: start outgoing shipments for a customer, article and volume

## Technologies

- Vue 3
- Vite for development and builds
- Ant Design Vue for the UI components and icons
- Axios for HTTP calls to the backend
- UUID for creating identifiers on the client

## Structure

- The project root holds the HTML entry page and the package manifest
- The src folder holds the application entry point, the root component and global styles
- The src/components folder holds the Warehouse component, which contains all the screens, forms and API calls
- The public folder holds static assets

## Status

This is a demo project from 2021 and is no longer maintained. It needs the matching CQRS warehouse backend running locally.