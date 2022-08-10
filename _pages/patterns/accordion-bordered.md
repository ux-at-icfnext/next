---
layout: pattern
categories: [patterns, accordion]
title: Bordered accordion
type: [detail-page]
permalink: /patterns/accordion/accordion-bordered/
description: |
    This variation of the accordion places a border around each open section. _For more information about how this component works, please read the specs for the [default accordion](/patterns/accordion/)._
overview: This variation of the accordion places a border around each open section.

usa-link: "https://designsystem.digital.gov/components/accordion/"

### Paths to view design and code... 
## designimg: can be used to show an image of the design until a coded version can be created. The htmlpath & csspath should be located in the pattens folder. Read more about creating coded components in /docs/creating-patterns 
# designimg: 
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
htmlpath: patterns/accordion/accordion-bordered.md
csspath: patterns/accordion/index.scss
---