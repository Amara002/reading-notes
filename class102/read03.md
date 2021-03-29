# Process and design of our website

**we have some rules that we should follow as**

- It's important to understand who your target audience is, why they would come to your site, what information they want to find and when they are likely to return.
- Site maps allow you to plan the structure of a site.
- Wireframes allow you to organize the information that will need to go on each page.
- Design is about communication. Visual hierarchy helps visitors understand what you are trying to tell them.
- You can differentiate between pieces of information using size, color, and style.
- You can use grouping and similarity to help simplify the information you present.

# HTML5 Layout

**we will know alot of tags to improve our website page which as follows:**

- < div > elements: to group together related elements.
- The < header > and < footer > elements can be used for: The main header or footer that appears at the top or bottom of every page on the site.
- The < nav > element: is used to contain the major navigational blocks on the site such as the primary site navigation.
- The < article > element: acts as a container for any section of a page that could stand alone and potentially be syndicated.
- The < aside > element: has two purposes, depending on whether it is inside an < article > element or not.
- The < section > element: groups related content together, and typically each section would have its own heading.
- The purpose of the < hgroup > element is to group together a set of one or more < h1 > through < h6 > elements so that they are treated as one single heading.
- The < figure > element: should also contain a < figcaption > element which provides a text decription for the content of the <figure> element. In this example, you can see a < figure > has been added inside 
the < article > element.
Examples of usage include:
    1. Images
    2. Videos
    3. Graphs
    4. Diagrams
    5. Code samples
    6. Text that supports the main body of an article
- Older browsers that do not know the new HTML5 elements will automatically treat them as inline elements. Therefore, to help older browsers, you should include the line of CSS on the left which states which new elements should be rendered as block-level elements.
as:
header, section, footer, aside, nav, article, figure 
{
display: block;} 
