---
layout: pattern
categories: [patterns, accordion]
title: Accordion
type: [sub-nav-item]
permalink: /patterns/accordion/
variations: true
overview:  An accordion is a list of headers that hide or reveal additional content when selected. They are helpful for keeping pages clean and easy to navigate.
description: |
    An accordion is a list of headers that hide or reveal additional content when selected. They are helpful for keeping pages clean and easy to navigate.

usa-link: "https://designsystem.digital.gov/components/accordion/"
specification: |
    In general, all accordions are closed on default. In some cases it maybe aventagious to have the first accordion in open state on load, but this technique should be used sparingly.

    #### Default Accordion
    - On click of a closed accordion bar, the accordion slides open to reveal the content inside, and the fa-plus icon switches to fa-minus. Any other open accordion will close.
    - On click of an open accordion bar, the accordion slides shut and the fa-minus icon is switched to the fa-plus.
    
    #### Multi-Select Accordion

    - On click of a closed accordion bar, the accordion slides open to reveal the content inside, and the fa-plus icon switches to fa-minus. Any other open accordion stays open.
    - On click of an open accordion bar, the accordion slides shut and the fa-minus icon is switched to the fa-plus.

    This component uses javascript functionality to work. Please see the documentation on USWDS for more information.
spec:
    - name: heading
      type: plain text
      class: usa-accordion__heading
      required: yes
      content: 80 characters
      example: "First Amendment"
      notes:
    - name: body
      type: plain text
      class: usa-accordion__content
      required: yes
      content: 500 characters
      example: |
        "Congress shall make no law respecting an establishment of religion, or prohibiting the free exercise thereof; or abridging the freedom of speech, or of the press; or the right of the people peaceably to assemble, and to petition the Government for a redress of grievances."
      notes:
    - name: button
      type:  button
      class: usa-accordion__button
      required: yes
      content: 20 characters
      example: "Find out more"
      notes:
designfile:
  - variable: accordion
    dataType: array
    desc: All accordion items that will be displayed.
  - variable: title
    dataType: string
    desc: Title of the accordion.
  - variable: content
    dataType: string
    desc: Content that will be included in the accordion.

accordion:
  - title: Accordion item 1
    content: accordion item 1 content
  - title: Accordion item 2
    content: accordion item 2 content
  - title: Accordion item 3
    content: accordion item 3 content

### Paths to view design and code... 
## designimg: can be used to show an image of the design until a coded version can be created. The htmlpath & csspath should be located in the pattens folder. Read more about creating coded components in /docs/creating-patterns 
# designimg: 
htmlpath: patterns/accordion/accordion.md
csspath: patterns/accordion/index.scss
---