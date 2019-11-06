# 3tiercss
Demo: https://lleadbet.github.io/3tiercss/

- [3tiercss](#3tiercss)
  - [Prerequisites](#prerequisites)
  - [Using this Repo](#using-this-repo)
  - [Designing Using this Framework](#designing-using-this-framework)
    - [Tier 1: Basscsss](#tier-1-basscsss)
    - [Tier 2: Making Things Twitchy](#tier-2-making-things-twitchy)
    - [Tier 3: Make It Your Own](#tier-3-make-it-your-own)
    - [Examples](#examples)


## Prerequisites 

To use this repo, you must have a SASS/SCSS compiler installed. We recommend using the one on [https://sass-lang.com/install](https://sass-lang.com/install) as it works quite well, and has a watch mode to test edits. 


Beyond that, a basic understanding of both SASS and CSS are strongly recommended to make the most out of this library.  

## Using this Repo

This repo has default colors and styles defined within the `/src/scss/partials` folder. We also have a local copy of [Basscss](https://basscss.com/) in the `/src/scss/vendor` folder as it is the basis for the customizations. 

To use this, simply create a new `.scss` file that first defines any color overrides using the variables, and then importing the `_base.css` partial. 

An example start file might look like:

```scss
/* Start: Color overrides */
$brand: #fff;
$brand-alt: #fff;
$accent: #fff000;

@import "partials/base";
/* Start: Class overrides */
...
```

Once you've written your SCSS, you can compile by doing: 

```sh
sass src/scss/:css/
```

You can also have it compile on changes by appending the `--watch` flag to the command, which is helpful during development. 

## Designing Using this Framework

This framework's design principles follow three tiers, described below. 

### Tier 1: Basscsss

This layer, being the easiest, is simply the Basscss framework available for you to use. This framework provides a number of helping classes, so take a look at the official site for more information: [Basscss](https://basscss.com/)

This tier is meant as a start point to build off of, and given the exceptionally small size, high functionality, and ease of use, we felt it a good place to base our changes off of. 

### Tier 2: Making Things Twitchy

The next tier is where Twitch is adding style to Basscss, making it feel more Twitch-y. This includes functionality like making buttons filled, improving the appearance of certain elements, and generally making things feel more modern. 

Basscss on it's own handles a lot of the fluidity of the UI, however it does not affect much of the actual appearance. This is the primary difference between the tiers- tier one is functional, tier two is design. 

### Tier 3: Make It Your Own

This tier is where you make it your own. You are now in full control of how it looks, given the foundation of both previous tiers. 

Working off of this, you are able to customize the appearance to a great extent while also leveraging the work already done by Twitch and Basscss. 

### Examples

For examples, see the demo site: https://lleadbet.github.io/3tiercss/readme.html

The code is available in the `/src/scss` folder for each of the provided examples, as well as compiled in the `/css` output folder. 
