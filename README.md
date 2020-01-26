# Recreation of Literatur und Kulturelles Leben poster

I chose this poster as it looked pretty complex, and I saw quickly what parts I could abstract into reusable css.

## Thoughts/Improvements

If I had more time, I can see that the light pink and light grey are textured - would have liked to have used a background image there to display the texture. Preferably a small texture image that can be repeated.

It looks like some of the columns have borders, if I did this again i'd like to implement that - they're quite inconsistent so I would probably have to add them to the 'rows'. I tried adding `border-right: 1px solid #8B747B;` but it looked way too harsh and didn't match the poster at all.

A lot of the columns are repeated. If I had more time I could have utilised nth-child for 'rows' and applied the height that way, so there are less css classes in the html and no need for having the heights applied inline.

I created a class for each different height, because I think having inline styles in your HTML is wrong and CSS should be kept seperate. This made an excessive amount of classes - again I think having a class for each type of column and applying the heights in the CSS using nth: child would have prevented this. If I was using a CSS compiler I could have further used variables to maintain all of the different height variants.

All of my CSS is in one file - preferably I would split these into their own SCSS components

I would have used flexbox, if it were compatible with IE 9 https://caniuse.com/#feat=flexbox
