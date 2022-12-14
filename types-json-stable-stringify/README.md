# Installation
> `npm install --save @types/json-stable-stringify`

# Summary
This package contains type definitions for json-stable-stringify (https://github.com/substack/json-stable-stringify).

# Details
Files were exported from https://github.com/DefinitelyTyped/DefinitelyTyped/tree/master/types/json-stable-stringify.
## [index.d.ts](https://github.com/DefinitelyTyped/DefinitelyTyped/tree/master/types/json-stable-stringify/index.d.ts)
````ts
// Type definitions for json-stable-stringify 1.0
// Project: https://github.com/substack/json-stable-stringify
// Definitions by: Matt Frantz <https://github.com/mhfrantz>
// Definitions: https://github.com/DefinitelyTyped/DefinitelyTyped

declare function stringify(obj: any, opts?: stringify.Comparator | stringify.Options): string;

declare namespace stringify {
    interface Element {
        key: string;
        value: any;
    }

    type Comparator = (a: Element, b: Element) => number;

    type Replacer = (key: string, value: any) => any;

    interface Options {
        cmp?: Comparator | undefined;
        space?: number | string | undefined;
        replacer?: Replacer | undefined;
    }
}

export = stringify;

````

### Additional Details
 * Last updated: Tue, 06 Jul 2021 21:33:48 GMT
 * Dependencies: none
 * Global values: none

# Credits
These definitions were written by [Matt Frantz](https://github.com/mhfrantz).
