# Horisen Code Refactor

## Horisen Ask

> Start: © 2020 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
```
AS A marketing agency
I WANT a codebase that follows accessibility standards
SO THAT our own site is optimized for search engines
```

## Acceptance Criteria
```
GIVEN a webpage meets accessibility standards
WHEN I view the source code
THEN I find semantic HTML elements
WHEN I view the structure of the HTML elements
THEN I find that the elements follow a logical structure independent of styling and positioning
WHEN I view the image elements
THEN I find accessible alt attributes
WHEN I view the heading attributes
THEN they fall in sequential order
WHEN I view the title element
THEN I find a concise, descriptive title
```
> End: © 2020 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.


## Changes Made to Horisen Code

### HTML
* title element changed from "website" to "Horisen"
* relevant div/span elements changed to semantic elements in order of appearance
  * header (header)
  * strong (seo in Horisen)
  * nav (nav links)
  * section (the services content)
  * article (each service listed)
  * aside (benefits side bar)
  * footer (footer)
  * small (copyright)
* alt attributes added to images with descriptions where relevant
* 'search-engine-optimization' nav link fixed by adding id to linked content
* shared class attribute added to service articles
* shared class attribute added to benefit divs
* .benefit h3s changed to h2s

### CSS
* eliminated redundant code by references new logical classes
  * for .service elements
  * for .benefit elements
* reordered code to follow html flow and group like sections
* added comments to search stylesheet more easily