# Module 1 Challenge: Code Refactor for Accessibility

## Description

This homework challenge dealt with refactoring working code to be more accessible. This involved adding semantic HTML tags to a messy set of "div" tags and subsequently changing CSS to reflect those changes. This work also involved fixing a broken link and changing the size of an image to fit the screen better. 
In the end, the final product is a more accessible html with proper alt tags on the images, and a throughly-commented and organized CSS page that is shorter then the original in code, but longer in descriptions of each section for ease of use in editing styles in the future.

## Procedure & Thought Process

This section details the procedure of refactoring the code, and the reasons I had behind each decision. Major changes are tracked here, smaller changes such as indentation and spacing are not discussed here.

### body 
    I began from the first children of the <body> tag first, replacing the <div>s with proper 
    semantic HTML tags.

    First comes a <div> with a class called "header". I removed the header class and replaced 
    it with the proper <header> tag.
 
    The next sibling <div> was one with the "hero" class. This class is defined in CSS as an
    image. 
    This declaration would be better written as a <figure> class alongside an <img> with a new, 
    more descriptive class name, thus the CSS "hero" class was removed. <figure>  replaced the 
    <div> with a "hero" class. Inside the <figure> tag contains the <img> tag with the class 
    "img-style", with a slightly altered src link to reflect the location of the html file and 
    proper alt text.

    The next sibling <div> was one with the "content" class. This will be replaced with the 
    <main> tag, as it contains the main content of the page, and the "content" class changed to 
    the <main> tag in CSS.

    The next sibling <div> was one with the "benefits" class. This is best replaced with the 
    <aside> tag, as this section serves as sidebar to the rest of the content. The "benefits" 
    class will be changed to an <aside> tag in CSS.

    The last sibling <div> was the one with the "footer" class. This will be replaced with the 
    proper <footer> tag. The "footer" class will be changed to <footer> tags in CSS.

### header

    Firstly, proper <nav> tags replaced the <div> tags containing the list of navigation 
    elements.
    
    Then, the "header div" with "nav" was removed in the CSS, as nav is its own element now
    
    The Search Engine Optimization nav link does not work. Looking at the syntax, each nav link 
    has an href with a # to an id in <main>. Thus, an id for "search engine optimization" was 
    added there.

### main

    There were 3 redundant classes, "search-engine-optimization," 
    "online-reputation-management" and "social-media-marketing" that had the same CSS code in 
    each. Thus, all three were replaced with one class, "section-style," truncating the CSS.

    <div> tags containing the id for the earlier navigation links and the "section-style" class 
    were replaced with the <article> tag, as each section could stand alone.

### aside

    Once again, the "benefit-lead," "benefit-brand," and "benefit-cost" classes have redundant 
    CSS. They will all be consolidated into the "sidebar-style" class.
    
    Chronologically, the <aside> code is after the <main> code. Thus, the "sidebar-style" CSS 
    code will be moved to be after the "section-style" CSS code.
    
    Each <div> in the sidebar can be replaced with the <section> tag, as these items could 
    stand alone. Arguably, <article> could work as well, as each heading, paragraph, and image 
    could stand alone, but without proper whitespace boundaries between each, <section> may fit 
    better.

### general finishing touches

    Alt text was added for all images. 
    Comments were added to all important sections of the HTML.
    Both CSS and HTML were validated through their respective online validators. No Errors were 
    detected.
    Comments were added to most sections of the CSS code, describing what each one changes and 
    styles.


## Screenshot of Final Product

    ![full screenshot of the horiseon website](assets/images/fullscreencap.png)

## Credits

I would like to thank MDN web docs at https://developer.mozilla.org/en-US/ for providing helpful references for code easily accessible within the VS code interface. This helped me figure out more troublesome parts of the CSS.

I also referenced tutorials on https://www.w3schools.com/ to help in implementing certain features, such as getting the proper image height. 

## Github Deployed Site Link and Repository Link

Github Repository: https://github.com/voravichs/1st-module-challenge
Github Pages Deployment: https://voravichs.github.io/1st-module-challenge/