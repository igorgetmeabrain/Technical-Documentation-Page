# Technical Documentation Page (freeCodeCamp challenge)

This project was created to fulfil an element of the Responsive Web Design course on freeCodeCamp.  
The main aim of the project is to create a documentation page, divided into multiple sections, navigated using a fixed navigation bar. The sections use code and li tags (amongst others) to organise content in a clear and easily digestible manner.

## Project Criteria

The required user stories are:  
1. I can see a main element with a corresponding id="main-doc", which contains the page's main content (technical documentation).
2. Within the #main-doc element, I can see several section elements, each with a class of main-section. There should be a minimum of 5.
3. The first element within each .main-section should be a header element which contains text that describes the topic of that section.
4. Each section element with the class of main-section should also have an id that corresponds with the text of each header contained within it. Any spaces should be replaced with underscores (e.g. The section that contains the header "JavaScript and Java" should have a corresponding id="JavaScript_and_Java").
5. The .main-section elements should contain at least 10 p elements total (not each).
6. The .main-section elements should contain at least 5 code elements total (not each).
7. The .main-section elements should contain at least 5 li items total (not each).
8. I can see a nav element with a corresponding id="navbar".
9. The navbar element should contain one header element which contains text that describes the topic of the technical documentation.
10. Additionally, the navbar should contain link (a) elements with the class of nav-link. There should be one for every element with the class main-section.
11. The header element in the navbar must come before any link (a) elements in the navbar.
12. Each element with the class of nav-link should contain text that corresponds to the header text within each section (e.g. if you have a "Hello world" section/header, your navbar should have an element which contains the text "Hello world").
13. When I click on a navbar element, the page should navigate to the corresponding section of the main-doc element (e.g. If I click on a nav-link element that contains the text "Hello world", the page navigates to a section element that has that id and contains the corresponding header.
14. On regular sized devices (laptops, desktops), the element with id="navbar" should be shown on the left side of the screen and should always be visible to the user.
15. My Technical Documentation page should use at least one media query.

The project is submitted via Codepen, using a CDN link to run tests to verify completion of the user stories:  
https://cdn.freecodecamp.org/testable-projects-fcc/v1/bundle.js  

## Design

This was my most ambitious submission to the FCC mini-projects. I chose to create a guide to solving a Rubik's Cube, as this fitted well with the required criteria for the project. I chose a bold colour-scheme which corresponds with that of a standard 3x3 cube. With a fixed navbar on the left, I kept the main content in the middle of the page and balanced the layout with an column of additional content on the right of the page.

Additional techniques which I explored in this project:
1. I explored CSS Grid as a technique for adjusting the layout when in portrait mode. In landscape (with fixed left navbar), the main content and additional content columns remained separate. In portrait, CSS Grid enabled me to intersperse the content from both columns into one full-width column, with the navbar fixed at the top of the screen instead.
2. I also used CSS Grid to create an animation to decorate the navbar. Creating a 3x3 grid, which responsively resizes, I used a colour-change animation to recreate the pattern of colours on the yellow face of a cube as a superflip algorithm is performed.
3. I had to use a more complex media query to entirely change the layout of the page for smaller screens. An additional intermediate media query was also used, to make content more legible for intermediate screen sizes.
4. I decided also to integrate basic spoilered text, with a clickable HINT button which reveals useful tips.
5. I realised that further animations would be necessary to make the guide as user-friendly as possible, but decided to integrate these in the form of an external user-customisable widget, as opposed to designing them from scratch myself.
6. Employing anti-headbutt tricks in portrait mode, to prevent content being hidden by the navbar when clicking on anchor tags.
7. In portrait mode, incorporating the main page title, animations and navlinks seamlessly into the navbar, whilst hiding an extraneous image, which was only useful for landscape orientation.
8. Again, I tried to make the layout and content of the page fully scalable, to cater for all possible screen sizes.

## Conclusion

The main challenges of this project were firstly to design and write the guide in a simple and appealing manner, suitable for novice cubers. All content on the page was written by me and all images were created (or modified from external sources) by me also. Secondly, to successfully rescale and reorient the layout for smaller screens (in portrait mode). This was tricky!
