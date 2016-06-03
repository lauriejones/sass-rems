# sass-rems

A SASS function for converting `px` to `rem`.

## Installation

    npm install --save sass-rems
    
## Usage

    $ sass-composer example/example.scss -o compiled.css

SCSS: `example/settings.scss`

    //this is the default setting if not specified by the user
    $base-font-size: 16px;
    

SCSS: `example/example.scss`
    
    @import "./settings";
    @import "sass-rems";

    h1 {
      padding: rem(15px);
      font-size: rem(24px);
    }

CSS: `compiled.css`

    h1 {
      padding: 0.9375rem;
      font-size: 1.5rem; }

## API

### rem($val, $ctx: $base-font-size)

Convert a `px` value to `rem`.

## License

The MIT License (MIT)

Copyright (c) 2015 James Newell