# PureJS_OnePageNav

The PureJS_OnePageNav library is designed to dynamically manage states of navigation links based on scroll offset. It comes with several options that allow customize page navigation working as intended.

Main functionalities:

-   dynamically update nav links accordingly to reached section
-   update hash accordingly to nav link or section
-   choosing which link should be default active if none section reached
-   exactly matching sections and no section zones with exact match option
-   allows to set classes on links parents like [li, nav], not only anchor tags
-   enforcing script loading only if suits defined URL paths
-   defining distance from top, at which section should be changed
-   visualization line for easier understanding
-   changing options after script initialization

## Getting Started

### Installation

```sh
npm install @zibuthe7j11/aperiam-et-quisquam
```

## Useful links

[Check out the demo](https://m-zoldak.github.io/PureJS_OnePageNav/demo/)

[Find more in Github wiki](https://github.com/m-zoldak/PureJS_OnePageNav/wiki/Configuration)

## Including into project and default values:

```js
import OnePageNav from '@zibuthe7j11/aperiam-et-quisquam';

// Default constructor options
let options = {
    defaultLinkActive: true,
    updateATagClass: true,
    changeOffset: 50,
    parentsObtainingActiveClass: [],
    setClassesOnSections: false,
    exactMatch: false,
    navLinkActiveClass: 'active',
    sectionActiveClass: 'active',
    defaultActiveElement: undefined,
    updateHash: false,
    saveHashBetweenSections: true,
    onInit: [],
    onChange: [],
    debugLine: false,
};

let onePageNav = new OnePageNav('nav a', options);

//or

new OnePageNav.default(); // for alone imported umd file
```

## License

#### The credit comments in the JavaScript files should be kept intact

(The MIT License)

#### Copyright (c) 2023 Mateusz Żołdak
