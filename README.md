# Registry

A web application similar to the official [npmjs.com](https://www.npmjs.com) website where users can search, view, and explore NPM packages. This TypeScript-based application consists of a homepage, a search results page, and a package details page.

## Features

-   **Search for NPM Packages**: Users can search for NPM modules using the search bar located in the header.
-   **Homepage**: The landing page contains a header with a logo and search bar, a brief description of the site, and a few example packages for users to explore.
-   **Search Page**: After submitting a search query, users are redirected to a search results page displaying relevant NPM packages based on the query.
-   **Package Details Page**: Users can view detailed information about a specific NPM package by clicking on the "View" button in the search results.

## Pages

1. **Homepage**:  
   The homepage includes:

    - A **header** that remains consistent across all pages, featuring:
        - A **logo** for branding.
        - A **search bar** to look up NPM modules.
    - A **landing section** with a title, description of the website, and example packages for quick access.

2. **Search Page**:  
   After a user enters a search query, they are redirected to this page. It displays:

    - A list of NPM packages that match the search query.
    - A **"View"** button next to each package, allowing users to navigate to the package details page.

3. **Package Details Page**:  
   This page provides detailed information about a selected package. Users can view:
    - Package name, description, version, and other relevant details.

## Technologies Used

-   **React**: The core library for building the UI.
-   **TypeScript**: Type safety throughout the application for a better development experience.
-   **React Router**: A full-featured navigation framework for implementing page routing.
-   **Tailwind CSS**: Utility-first CSS framework used for styling the user interface.
-   **React Icons**: Popular icons that can be used in React projects.

## Project Structure

-   **/src**
    -   **/components**
        -   Header.tsx - Header component with logo and search bar.
        -   PackageListItem.tsx - Package list item component.
        -   SearchIput.tsx - Displays search field.
    -   **/page**
        -   **/home**
            -   HomePage.tsx
            -   homeloader.ts
        -   **/details**
            -   DetailsPage.tsx
            -   detailsLoader.ts
        -   **/search**
            -   SearchPage.tsx
            -   searchLoader.ts
        -   Root.tsx
    -   **/api**
        -   **/queries**
            -   getFeaturedPackages.ts
            -   getPackage.ts
            -   searchPackages.ts
        -   **/types**
            -   packageDetails.ts
            -   packageSummary.ts
    -   App.tsx - Main app component.

## How It Works

1. **Search for Packages**:

    - A user can type a search term (e.g., `react`) into the search bar located in the header and press Enter.
    - They are redirected to the **Search Page** where relevant NPM packages are displayed.

2. **View Package Details**:
    - From the search results, users can click the **View** button next to a package to navigate to the **Details Page**.
    - The package details, including its name, description, version, and more, are displayed.

## Installation and Setup

1. **Clone the repository**:

    ```bash
    https://github.com/olaide-hok/Registry.git
    ```

2. **Install dependencies**:

    ```bash
    npm install
    ```

3. **Start the development server**:

    ```bash
    npm start
    ```

4. **Open in your web browser**: Visit <http://localhost:5173> to interact with the map and search features.
