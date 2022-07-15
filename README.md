# 1st-module-challenge
As I progress through each step, the page was reloaded to make sure it looks the same after semantic changes. Thus, some incremental steps may skip ahead to ensure this occurs.

<body>
I began from the first children of the <body> tag first, replacing the <div>s with proper semantic HTML tags.

    First comes a <div> with a class called "header". I removed the header class and replaced it with the proper <header> tag.
 
    The next sibling <div> was one with the "hero" class. This class is defined in CSS as an image. This declaration would be better written as a <figure> class alongside an <img> with a new, more descriptive class name, thus the CSS "hero" class was removed. <figure>  replaced the <div> with a "hero" class. Inside the <figure> tag contains the <img> tag with the class "img-style", with a slightly altered src link to reflect the location of the html file and proper alt text.

    The next sibling <div> was one with the "content" class. This will be replaced with the <main> tag, as it contains the main content of the page, and the "content" class changed to the <main> tag in CSS.

    The next sibling <div> was one with the "benefits" class. This is best replaced with the <aside> tag, as this section serves as sidebar to the rest of the content. The "benefits" class will be changed to an <aside> tag in CSS.

    The last sibling <div> was the one with the "footer" class. This will be replaced with the proper <footer> tag. The "footer" class will be changed to <footer> tags in CSS.

header

    Added proper nav tags
    removed "header div" with "nav" as nav is its own element that can be referred to
    the Search Engine Optimization nav link does not work. Looking at the syntax, each nav link has an href with a # to an id in <main>. Thus, an id for "search engine optimization" was added there.

main

    There were 3 redundant classes, "search-engine-optimization," "online-reputation-management," and "social-media-marketing" that had the same CSS code in each. Thus, all three were replaced with one class, "section-style," truncating the CSS.
    <div> tags containing the id for the earlier navigation links to reference and the "section-style" class were replaced with the <article> tag, as each section could stand alone.

aside

    Once again, the "benefit-lead," "benefit-brand," and "benefit-cost" classes have redundant CSS. The will all be consolidated into the "sidebar-style" class.
    Chronologically, the <aside> code is after the <main> code. Thus, the "sidebar-style" CSS code will be moved to be after the "section-style" CSS code.
    Each <div> in the sidebar can be replaced with the <section> tag, as these items could stand alone. Arguably, <article> could work as well, as each heading, paragraph, and image could stand alone, but without proper whitespace boundaries between each, <section> may fit better.
