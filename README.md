# Angular 18 with ng-bootstrap Demo

This project demonstrates the integration of Angular 18.2.1 with ng-bootstrap, utilizing the traditional module-based approach instead of standalone components.

## Project Overview

- **Angular Version**: 18.2.1
- **Bootstrap Version**: 5.3.3
- **ng-bootstrap**: Latest compatible version

This demo showcases how to integrate and use ng-bootstrap components in an Angular 18 application without employing standalone components.

## Prerequisites

Before you begin, ensure you have the following installed:
- Node.js (LTS version recommended)
- npm (comes with Node.js)

## Getting Started

To get the project up and running on your local machine, follow these steps:

1. Clone the repository:

```sh
git clone [repository-url]
cd angular-18-bootstrap
```

2. Install dependencies:

```sh
npm install
```
3. Start the development server:

```sh
ng serve
```

4. Open your browser and navigate to `http://localhost:4200/`. The application should be running.

## Project Structure

The project follows the standard Angular project structure:

src/
├── app/
│   ├── components/
│   ├── app.component.ts
│   ├── app.component.html
│   ├── app.module.ts
│   └── ...
├── assets/
├── environments/
├── index.html
└── ...

## Features

- Demonstrates the use of various ng-bootstrap components
- Showcases Angular 18 features
- Utilizes Bootstrap 5.3.3 for styling

## Usage Examples

Here's a basic example of using an ng-bootstrap component in this project:

```html
<button
  class="btn btn-outline-secondary"
  placement="bottom"
  [ngbPopover]="popoverContent"
  popoverTitle="Choose format"
>
  Popover with format options
</button>

<ng-template #popoverContent>
  <div class="d-flex flex-column">
    <button class="btn btn-sm btn-outline-primary mb-2">SVG</button>
    <button class="btn btn-sm btn-outline-primary mb-2">PNG</button>
    <button class="btn btn-sm btn-outline-primary">PDF</button>
  </div>
</ng-template>
