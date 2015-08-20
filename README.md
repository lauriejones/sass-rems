# sass-ems

A SASS function for converting `px` to `em`.

## Installation

    npm install --save sass-ems
    
## Usage

    $ sass-composer example/example.scss -o compiled.css

SCSS: `example/example.scss`
    
    @import "sass-ems";
    
    $base-font-size: 16px; //defaults to 16px if not set
    
    h1 {
      padding: em(15px);
      font-size: em(24px);
    }

CSS: `compiled.css`

    h1 {
      padding: 0.9375em;
      font-size: 1.5em; }

## API

### em($val, $ctx: $base-font-size)

Convert a `px` value to `em`.

## License

The MIT License (MIT)

Copyright (c) 2015 James Newell