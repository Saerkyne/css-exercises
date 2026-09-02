# An entire page!

Flexbox is useful for laying out entire pages as well as the smaller components we've already been working with. For this exercise, we're leaving you with a little more work to do, with some things you may not have encountered yet. It's perfectly acceptable to google things you're unsure of!

### Hints
- You may want to search something like `CSS remove list bullets`.  We've done this for you in previous examples, but not here. Yay learning.
- Finding out how to style links in CSS might help you get rid of that pesky underline decoration...
- We've added `height: 100vh` to the `body`... this makes the body exactly the same height as the viewport. To stick the footer to the bottom you will need to use flex and change the direction to column.

## Desired Outcome
![desired outcome](./desired-outcome.png)

### Self Check

- The header is at the top of the page, the footer is at the bottom, and they stay in place if you resize your screen.
- The header and footer have padding.
- The links in the header and footer are pushed to either side.
- There is space between the links in the header and footer.
- The footer has a light gray background (`#eeeeee`).
- The logo, input and buttons are centered in the screen.
- The buttons have an appropriate amount of padding.
- There is space between the logo, input and buttons.


## UPDATE
So my solution works, but is different from the shown one again. I didn't combine repeat styles into a single section, and I have a habit of putting padding on individual flex items instead of on the flex container. For example, I added a top and bottom margin to the input bar, whereas the solution added a padding to the buttons and a gap to the content box. I also used align-self on the content container and that seems to be unnecessary. I also added a max-height constraint to the header and footer and a justify-content: flex-end for right side links where it was unnecessary. 

It works, but not as cleanly as the solution. There's a lot of extra, messy styling here. 