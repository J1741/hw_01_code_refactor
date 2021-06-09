# Overview
This file describes changes during a recent project to refactor the codebase for the Horiseon Social Solution Services website for better accessibility and SEO.

# Requirements

## User Story
The Horiseon refactoring project targeted the following user story:

```
AS A marketing agency
I WANT a codebase that follows accessibility standards
SO THAT our own site is optimized for search engines
```

## Acceptance Criteria
The following acceptance criteria were identified as requirements for successful completion of the Horiseon refactoring project:

```
1. WHEN I view the source code
- THEN I find semantic HTML elements

2. WHEN I view the structure of the HTML elements
- THEN I find that the elements follow a logical structure independent of styling and positioning

3. WHEN I view the image elements
- THEN I find accessible alt attributes

4. WHEN I view the heading attributes
- THEN they fall in sequential order

5. WHEN I view the title element
- THEN I find a concise, descriptive title

6. WHEN I click a link on the page
- THEN it works correctly

7. WHEN I view the source code
- THEN all CSS selectors and properties
  -- are consolidated
  -- and follow a semantic structure

8. WHEN I view the source code
- THEN the CSS file is properly commented
```

# File Changes

## HTML
To fulfill the above requirements, the following changes were made in the codebase HTML file: `./index.html` 

- Acceptance criteria were added to the HTML for reference
- The `<title>` element content was updated to "Horiseon Social Solution Services"
- Alt attributes with informative descriptions were added to all `<img>` elements
- A broken navigation link to the "Search Engine Optimization" section was repaired 
- Semantic elements were added to the HTML file to increase accessibility and SEO:
  - All existing `<div>` elements were replaced semantic ones, or adding new semantic elements entirely
  - In some cases, new semantic elements were added to add a more thematic and/or logical structure to the HTML
  - Semantic elements in the refactored HTML include: `<header>, <nav>, <section>, <figure>, <main>, and <aside>`
  - **NB:** A `<footer>` element was briefly added to the HTML, but was then removed, as a footer was not present in the refactoring mock-up
- Heading `<h2>` tags were re-ordered within the `<main>` `<section>` elements to appear before the rest of the section content
- Custom classes were added to two `<h2>` elements to support precise placement relative to the images in their sections
- Comments tracking changes made during refactoring were made throughout the HTML file

## CSS
To fulfill the above requirements, the following changes were made in the codebase CSS file: `./assets/css/style.css`
- Comments, comment sections, and a table of contents were added to summarize styles and make the file easier to navigate
- Repetitive CSS selectors and properties were consolidated into single styles
- `<img>` element placement and heading margins were tweaked to accommodate reorganization of some `<h2>` tags in the HTML (see above)
- The height of the `<section>` elements within `<main>` was reduced to make the deployed application match the mockup
- A margin was added below the `<aside>` element to make the deployed application match the mockup
- **NB:** A footer style was originally added to the CSS, but was then removed, as a footer was not present in the refactoring mockup
- Comments tracking changes made during refactoring were made throughout the HTML file 

# Deployed Application

## Link to Deployed Application
The following link can be followed to access the deployed application:
https://j1741.github.io/hw_01_code_refactor/

## Screenshot of Deployed Application
The following screenshot of the deployed application illustrates the results of the refactoring project:

![Alt text](./screenshot.png?raw=true "Screenshot After Refactor")