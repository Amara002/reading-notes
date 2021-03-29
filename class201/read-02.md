# Text
***When creating a web page, you add tags (known as markup) to the contents of the page. These tags provide extra meaning and allow browsers to show users the appropriate structure for the page.***

## Heading
**HTML has six "levels" of headings:'< h1>' is used for main headings'< h2>-----< h6>' are used for subheadings**

## paragraph
**To create a paragraph, surround the words that make up the paragraph with an opening '< p>' tag and closing '< /p>' tag.**

## Bold & Italic
- **By enclosing words in the tags '< b>' and '< /b>' we can make characters appear bold.**
- **By enclosing words in the tags '< i>' and '< /i>' we can make characters appear italic.**

## Superscript & Subscript
- **The '< sup>' element is used to contain characters that should be superscript such as the suffixes of dates or mathematical concepts like raising a number to a power such as 2<sup>2</sup>.**
- **The '< sub>' element is used to contain characters that should be subscript. It is commonly used with foot notes or chemical formulas such as H<sub>2</sub>o.**

## Line break & horizontal rules
- **'< br />':As you have already seen, the browser will automatically show each new paragraph or heading on a new line. But if you wanted to add a line break inside the middle of a paragraph you can use the line break tag '< br />'.**
- **'< hr />'To create a break between themes — such as a change of topic in a book or a new scene in a play — you can add a horizontal rule between sections using the '< hr />' tag.**

## Semantic mark up
***There are some text elements that are not intended to affect the structure of your web pages, but they do add extra information to the pages — they are known as semantic markup.***

### Strong & Emphasis
- **'< strong>': The use of the '< strong>' element indicates that its content has strong importance.**
- **'< em>': The '< em>' element indicates emphasis that subtly changes the meaning of a sentence.**
### Quotations
- **'< blockquote>': The '< blockquote>' element is used for longer quotes that take up an entire paragraph. Note how the '< p>' element is still used inside the '< blockquote>' element.**
- **'< q>': The '< q>' element is used for shorter quotes that sit within a paragraph.**
### Abbreviations & Acronyms
**If you use an abbreviation or an acronym, then the '< abbr>' element can be used. A title attribute on the opening tag is used to specify the full term.**
### Citations & Definitions 
- **'< cite>': When you are referencing a piece of work such as a book.** 
- **'< dfn>': The first time you explain some new terminology (perhaps an academic concept or some jargon) in a document.**
### Author Details
**'< address>': The '< address>' element has quite a specific use, to contain contact details for the author of the page.**

# Introducing CSS
***CSS allows you to create rules that specify how the content of an element should appear.***

## CSS Associates Style rules with HTML elements
**CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. A CSS rule contains two parts: a selector and a declaration.**
## Using External CSS
***The '< link'> element can be used in an HTML document to tell the browser where to find the CSS file used to style the page. It is an empty element (meaning it does not need a closing tag), and it lives inside the '< head>' element. It should use three attributes:***
- **href: This specifies the path to the CSS file (which is often placed in a folder called css or styles).**
- **type: This attribute specifies the type of document being linked to. The value should be text/css.**
- **rel: This specifies the relationship between the HTML page and the file it is linked to. The value should be stylesheet when linking to a CSS file.**

## CSS Selectors
**We can know them from this**[figure](selectors.PNG)

# Basic Javascript instructions
***instructions you want it to follow as:***
- **THE LANGUAGE SYNTAX AND GRAMMAR: like any new language, there are new words to learn (the vocabulary) and rules for how these can be put together (the grammar and syntax of the language).**
- **GIVING INSTRUCTIONS: FOR A BROWSER TO FOLLOW Web browsers (and computers in general) approach tasks in a very different way than a human might. Your instructions need to reflect how computers get things done.**

## Statments
***A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a statement. Statements should end with a semicolon.***
## Comments
***You should write comments to explain what your code does. They help make your code easier to read and understand. This can help you and others who read your code.***
## Variables
***A script will have to temporarily store the bits of information it needs to do its job. It can store this data in variables.*** 
