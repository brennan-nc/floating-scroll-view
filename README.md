floating-scroll-view
====================

An attempt at creating a floating scroll view, centered vertically, in autolayout.

The idea is that we have content with absolute size, so the scrollview that contains it knows its size. The scrollview that contains it should know it needs to be exactly this size. The scrollview is in turn in a container, which it is aligned perfectly within (in theory there could be content above and below the scroll view). This content container is then aligned vertically within the root container, and it has some amount of set leading and trailing space.

The idea is a modal pop-over box with dynamically sized content in the scrollview that is always vertically centered (the height would max at the screen height, but that detail is irrelevant for the general problem). However, the layout doesn't even seem possible with the size of the scrollable content known, as per this example.

Expected:
![alt tag](https://github.com/brennan-nc/floating-scroll-view/blob/master/ReadmeImages/photo1.jpg)
