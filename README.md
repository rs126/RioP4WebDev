# M.5.2 Lab Accessibility

This is a starter project for web development with no frameworks and minimal
dependencies.It is intended to be a starting point for web development projects
that are written in plain HTML, CSS, and JavaScript. 
For this project, we attempted to increase the accessibility of a given website.


## Getting Started

To get started, clone this repository and run the following commands:

```bash
npm install
```
This will install the necessary dependencies for the project.

## Development

It is recommended to use the VSCode Live Server extension to run the project
locally. This will allow you to see changes in real-time as you make them. There
is no need to run a build process or refresh the page manually. Additionally,
you do not need to setup a local server to run the project.

When Live server is installed you can access it by clicking on index.html, then on the square icon
with the magnifying glass at the top right of the screen.

Additionally, you can copy and paste the URL live server gives you into the browser window.

## Testing

Note: there are tests but they will not work for this particular project. They are remnants from the template
repository.

To run the tests for the project, run the following command:

```bash
npm test
```

## Accessiblity Lab Answers

### Color
Contrast is known as the ratio between the darkest black and brightest whites. It is possible to test the contrast of a webpage using Google Chromes Dev Tools. The process for this involves right clicking then clicking inspect. At the top left of the window that pops up there should be a selector where you can click elements on a webpage and it will show you the calculation. In my case the Contrast was 2.79. It recommended changing the color of the font to white. But instead to match the assignment guidelines I changed the background color of the nav divs  to white.

### Semantic HTML

1. When using a keyboard it appears that you can navigate through the webpage as you would a normal website. By default I can use the arrow keys or sometimes the space bar to scroll up and down. Or I can use the tab key to navigate to the header and other interactive elements.
2.  From what I have seen to make screen readers have an easier time navigating your article, you should either make use of proper sematic HTML or use ARIA roles. In my case I use sematic HTML and added proper headings, paragraph tags and attributes like alt text for image tags to make screen reader navigation simpiler.
3. It turns out that the navigation menu should actually be nested in a `<nav>` element as opposed to a `<div>`. This is because this tag was designed to hold navigation links.

### Images

To be accessible to a screen reader you need to add alt text to the image.

### The Audio Player

1. An accessible alternative I added for hearing impaired users is a button that will show and hide the transcript.

2. In the instance that the HTML audio player isn't accessible to those using older browsers, I have provided a link to download the audio file so the end user can still access it.

### The Forms

1. To add a label that is only accessible to screen readers you can add the aria-label property to the input element. Then when the users click the box its purpose will be stated by the screen reader.

2. To make the `<input>` elements unambiguously associated with thier labels. you have to nest the inputs in a label tag and update their for attribute.

### The Show/Hide Comment Control
You can make the Show/Hide comments button keyboard accessible by making it a `<button>` instead of a `<div>` element. With this approach the enter key will also work for activating it.

### The table

From what I have seen, something that may help screen readers to identify rows and columns is to use proper sematic elements. As an example proper use of the `<th>` and `<td>` elements in table code. Also the proper use of the `scope` attribute to identify rows an columns.

### Other Considerations

One consideration for accessibility would be to make the interface completely responsive to the viewport. So its usable and looks visually appealing on any device including phones, or laptops with much smaller screens.

Another consideration to improve accessibility is to make it so elements that require input or elements in the navbar, have different colored border around them when your mouse hovers over them. This will make it so users can more easily identify where they are and what they might be able to click on in the webpage.


## Citations

“HTML: A Good Basis for Accessibility - Learn Web Development | MDN.” MDN Web Docs, 12 Aug. 2025, https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Accessibility/HTML.

“ARIA: Form Role - ARIA | MDN.” MDN Web Docs, 7 Jun. 2025, https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Reference/Roles/form_role.

Mozilla. :“:Focus-Visible - CSS | MDN.” MDN Web Docs, 14 Jul. 2025, https://developer.mozilla.org/en-US/docs/Web/CSS/:focus-visible.

HTML Caption Tag. https://www.w3schools.com/tags/tag_caption.asp. Accessed 21 Sep. 2025.

HTML Th Scope Attribute. https://www.w3schools.com/tags/att_th_scope.asp. Accessed 21 Sep. 2025.









