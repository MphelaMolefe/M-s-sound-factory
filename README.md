# M's Sound Factory

A colorful, responsive static website for M's Sound Factory, an audio and sound production business.

The site is built with plain HTML, CSS, and browser JavaScript. It does not require a package manager, build tool, or framework.

## Features

- Shared navigation across all website pages
- Colorful responsive design
- Full-screen background video
- Background video configured to autoplay, stay muted, loop continuously, and play inline on mobile
- Speaker and audio imagery from the local assets folder
- About Us content and team information
- Services page with three service sections and images
- Contact form
- Enquiry form
- Live local time display on the Contact page
- Embedded Google Map for:
  - 123 Main Street, Polokwane, Limpopo, South Africa
- Google Maps directions link
- Accessible labels, alternative image text, navigation labels, and reduced-motion support
- Responsive layouts for desktop and mobile screen sizes

## Project Structure

```text
part 1/
|-- README.md
|-- assests/
|   |-- image 1.jpeg
|   |-- image 2.jpeg
|   |-- image 3.jpeg
|   |-- WhatsApp Video 2026-09-18 at 19.33.39.mp4
|-- css/
|   |-- style.css
|-- html/
|   |-- home.html
|   |-- home-details.html
|   |-- about-us.html
|   |-- services.html
|   |-- enquiry.html
|   |-- contact.html
|-- .vscode/
    |-- settings.json
```

## Pages

| Page | File | Purpose |
| --- | --- | --- |
| Home | `html/home.html` | Main landing page with the site introduction and image |
| Home Details | `html/home-details.html` | Company introduction and feature information |
| About Us | `html/about-us.html` | Company information, values, vision, and team |
| Services | `html/services.html` | Service sections with local images |
| Enquiry | `html/enquiry.html` | Enquiry form |
| Contact | `html/contact.html` | Contact form, live clock, address, map, and directions |

Every page uses the shared navigation menu with links to Home, About Us, Services, Enquiry, and Contact.

## How To Run

### Option 1: Open directly

Open `html/home.html` in a modern web browser.

The local HTML, CSS, images, and video work without a build step.

### Option 2: Use VS Code Live Server

1. Open the project folder in VS Code.
2. Install the **Live Server** extension if it is not already installed.
3. Right-click `html/home.html`.
4. Select **Open with Live Server**.

Using a local server is recommended because browser security settings may restrict embedded content or local media when files are opened directly.

### Option 3: Use a simple local server

From the project root, run one of the following commands:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000/html/home.html
```

## Styling

All pages use:

```html
<link rel="stylesheet" href="../css/style.css">
```

The shared stylesheet contains:

- Color variables and page-wide theme rules
- Responsive navigation
- Cards, forms, buttons, images, and map styling
- Background video positioning and overlays
- Page-load animations and hover interactions
- Mobile breakpoints
- Reduced-motion support through `prefers-reduced-motion`

## Background Video

Each page loads this local video:

```text
assests/WhatsApp Video 2026-09-18 at 19.33.39.mp4
```

The video is used as a fixed background with these attributes:

```html
<video autoplay muted loop playsinline>
```

The CSS places it behind the page content and adds a translucent overlay so text remains readable.

## Contact Page

The Contact page includes:

- Live local time updated every second with JavaScript
- Email address: `M'ssound@gmail.com`
- Phone number: `+27 12 345 6789`
- Address: `123 Main Street, Polokwane, Limpopo, South Africa`
- Google Maps embed
- Google Maps directions link

An internet connection is needed for the embedded Google Map and external directions link.

## Forms

The forms currently use these actions:

```text
submit_contact.php
submit_enquiry.php
```

Those PHP handler files are not included in this static project. The forms will display correctly, but successful server-side submission requires a PHP backend or another form-processing service to be added.

## Accessibility

The project includes:

- Semantic HTML structure
- Descriptive page titles
- Labels connected to form controls
- Alternative text for images
- Navigation labels using `aria-label`
- Live clock updates using `aria-live="polite"`
- A descriptive map iframe title
- `prefers-reduced-motion` support

## Browser Support

Use a current version of:

- Google Chrome
- Microsoft Edge
- Mozilla Firefox
- Safari

Background video autoplay depends on browser policy. It is muted intentionally so browsers allow autoplay without user interaction.

## Maintenance Notes

- Keep all HTML pages inside `html/`.
- Keep the shared stylesheet inside `css/style.css`.
- Keep images and video inside `assests/`.
- Use relative paths from each HTML page when adding new assets.
- Update the navbar on every page when adding or renaming a page.
- Use a local server when testing maps, media, and future backend integrations.

M's Sound Factory Website
Student Information
Name: Mphela Molefe
Student Number: ST10529130
Module: WEDE5020 - Web Development (Introduction)
Qualification: Diploma in Information Technology
Institution: The Independent Institute of Education (IIE)
Submission: Part 1

Project Overview
M's Sound Factory is a professional audio service business that specialises in providing high-quality sound equipment and technical support for events. The company offers sound hire services for weddings, conferences, parties, live performances, corporate events, and other special occasions.
The purpose of this website is to establish an online presence for the business, showcase available services, provide company information, and allow potential clients to make enquiries regarding sound equipment rental and event support services.
This project follows the Web Development module requirements and will be developed over three parts, with new features and improvements added throughout the development process.

Website Goals and Objectives
Goals
* Create a professional online presence for M's Sound Factory.
* Increase brand awareness and visibility.
* Showcase available sound equipment and services.
* Provide contact information for client enquiries.
* Improve customer engagement through an easy-to-use website.
Objectives
* Develop a user-friendly website structure.
* Present clear information about services offered.
* Ensure responsive and accessible design principles are followed.
* Create a professional visual identity.
* Prepare the website for future interactive functionality.

Key Features and Functionality
Home Page
* Introduction to M's Sound Factory.
* Overview of services.
* Business highlights and promotional content.
About Us Page
* Company background.
* Mission and vision statement.
* Business values.
Services Page
* Detailed descriptions of available sound services.
* Equipment rental information.
Gallery Page
* Images of previous events and equipment setups.
Contact Page
* Contact details.
* Business location information.
* Enquiry form (to be implemented in later parts).

Timeline and Milestones
PhaseActivityStatusWeek 1Business selection and planningCompleteWeek 2Research and content gatheringCompleteWeek 3Website structure planningCompleteWeek 4Part 1 documentationCompletePart 2HTML development and implementationPendingPart 3Styling, testing and refinementsPending
Part 1 Details
Completed Tasks
1. Business Selection
Selected M's Sound Factory as the business for the website project.
2. Research
Gathered information regarding:
* Business services
* Target audience
* Industry requirements
* Competitor analysis
3. Website Planning
Planned:
* Website purpose
* Website goals
* Target audience
* Website content structure
4. Information Architecture
Created the sitemap and page structure for future development.

Sitemap
Home
?
??? About Us
?
??? Services
?
??? Gallery
?
??? Contact Us

Changelog
Version 1.0 - Part 1 Submission
Added
* Project overview
* Website goals and objectives
* Business information
* Initial sitemap
* Website planning documentation
* Timeline and milestones
Planned for Part 2
* HTML page creation
* Navigation menu
* Content implementation
* Images and media integration
Planned for Part 3
* CSS styling
* Responsive design
* Website testing
* Final refinements

References
The Independent Institute of Education. (2026). WEDE5020 Web Development (Introduction) Module Manual. The Independent Institute of Education.
MDN Web Docs. (2026). HTML: HyperText Markup Language. Available at: https://developer.mozilla.org/ [Accessed Day Month Year].
MDN Web Docs. (2026). CSS: Cascading Style Sheets. Available at: https://developer.mozilla.org/ [Accessed Day Month Year].
W3Schools. (2026). HTML Tutorial. Available at: https://www.w3schools.com/html/ [Accessed Day Month Year].
W3Schools. (2026). CSS Tutorial. Available at: https://www.w3schools.com/css/ [Accessed Day Month Year].

Author
Mphela Molefe
ST10529130
2026
