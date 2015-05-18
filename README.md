# rowlow.utils.breakpoints

Defining a map of breakpoint names and value pairs, this module generates will help you maintain responsive breakpoints for your project. By default, this module will give you breakpoints at 1px, 768px, 992px and 1200px.

## Install

```
    bower install --save rowlow.utils.breakpoints
```

## Variables

```
    $rowlow-breakpoints: (
        "s":    1,
        "m":    768,
        "l":    992,
        "xl":   1200
    );
```

## Functions
```
    rowlow-breakpoint()         // Returns a breakpoint value by a given name
    rowlow-breakpoint-min()     // Returns the breakpoint's min value by a given name
    rowlow-breakpoint-max()     // Returns the breakpoint's max value by a given name
```

## Usage

### Setup
```
    /* Overwrite breakpoint map (optional) */
    $rowlow-breakpoints: (
        "s":    1,
        "m":    992,
        "l":    1200,
        "xl":   1400,
        "xxl":  1600
    );

    @import "bower_components/rowlow.utils.breakpoints/main.scss"
```

### SCSS
```
    @media (min-width: rowlow-breakpoint-min("s") + px) {

    }

    @media (min-width: rowlow-breakpoint-min("m") + px) {
        
    }

    @media (min-width: rowlow-breakpoint-min("l") + px) {
        
    }

    @media (min-width: rowlow-breakpoint-min("xl") + px) {   

    }
```

