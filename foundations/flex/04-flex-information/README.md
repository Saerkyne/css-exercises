# A very common website feature

The goal of this exercise is to recreate a section that is found on many informational websites.

For this one you will need to edit the HTML a little bit too. We can't be making things _too_ easy for you. You'll want to add containers around the various elements so that you can flex them. Good luck!

## Desired outcome

![desired outcome](./desired-outcome.png)

### Self Check

- All items are centered on the page (horizontally, not vertically).
- The title is centered on the page.
- There is 32px between the title and the 'items.'
- There is 52px between each item.
- The items are arranged horizontally on the page.
- The items are only 200px wide and the text wraps.
- The item text is centered.


## RESULTS
My code worked up until I resized the window I was looking at. Then it failed and the flexboxes lined up incorrectly. interestingly, I had way more added code to the stylesheet and most of it didn't work. I was aiming for scalable, this wanted fixed placement and margins. Here's what was different: 

body {
    I set display: flex and set up flex-wrap: wrap. Solution just had text-align: center.
}

.title {
    I had text-align: center here, with a flex-basis of 100% to allow for full width since I made the whole body a flex box. I added a 32px padding-bottom. 

    Solution just had a margin-bottom of 32px. 
}

.container (I called this .information) {
    I set a display: flex and a gap of 52px. 

    Solution did the same, but put centered justify-content here instead of on the items themselves. This is where I messed up my placement. 
}

.info (I called this .item) {
    I put justify-content: center here, with flex: 1, display: flex; and flex-wrap since when I did this on the specific window size I was working in it seemed to work. 

    Solution only has a max-width of 200px set here. 
}

.text {
    I set width of 200px and text-alignment here, but it was unneeded with the solution setup. 

    Solution didn't do anything witht he text class. 
}