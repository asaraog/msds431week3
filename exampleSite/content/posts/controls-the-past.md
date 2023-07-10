---
title: Markdown is inaccessible
date: 2022-05-05
description: "Markdown, as a text-based markup language, can present challenges in terms of accessibility for individuals with disabilities. Here are some reasons why Markdown can be considered inaccessible."
image: images/Markdown.svg
imageAltAttribute: Markdown
tags:
   - markdown
   - accessibility 
   - ChatGPT
---

## Markdown in Obsidian

Markdown, as a text-based markup language, can present challenges in terms of accessibility for individuals with disabilities. Here are some reasons why Markdown can be considered inaccessible:

1. Lack of Structural Information: Markdown's simplicity and lightweight syntax often result in a lack of structured information within the document. Accessibility relies on proper semantic structure, such as headings, lists, and tables, which aid in navigation and comprehension for individuals using assistive technologies like screen readers. Without these structural elements, understanding the hierarchy and organization of content becomes difficult for those who rely on assistive technology.

2. Limited Support for Alternative Text: Alternative text (alt text) is crucial for providing descriptions of images and other visual elements to individuals who are blind or visually impaired. While Markdown does support image insertion, it doesn't inherently provide a way to add alt text. Users must rely on external tools or additional markup to add descriptive alt text, making the process more complex and error-prone.

3. Absence of ARIA Roles and Attributes: Accessible Rich Internet Applications (ARIA) roles and attributes help enhance the accessibility of web content. However, Markdown lacks direct support for adding ARIA roles and attributes to elements. These attributes provide valuable information to assistive technologies, enabling better interaction and comprehension for users with disabilities.

4. Limited Styling and Customization Options: Markdown's focus on simplicity often restricts the available styling options. While this simplicity aids readability, it can also limit the ability to customize text for improved accessibility. Accessibility often involves adjusting color contrast, font sizes, and other visual properties to meet specific needs. Markdown's limited styling capabilities may not adequately support these requirements.

5. Complex Table Accessibility: Tables are commonly used to organize and present data. However, creating accessible tables in Markdown can be challenging due to the lack of dedicated syntax for table headers, captions, and summary attributes. Ensuring proper table semantics and associating data cells with headers requires additional effort and manual markup modifications.

It's important to note that while Markdown may have inherent accessibility limitations, these challenges can be addressed by combining Markdown with additional HTML markup and accessibility practices. By carefully considering the accessibility needs of users and employing appropriate techniques, it is possible to create more accessible content with Markdown.

Source: ChatGPT "give me a description why Markdown is inaccessible"