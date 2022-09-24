# Hello World Test Application

This is just a simple GUI-based Hello World application for the Flipper Zero. It draws a border, places text that says "Hello World!" somewhere on the screen, and moves it around. Pressing the arrow buttons increases or decreases the amount in the x or y axis the text moves per tick. Pressing enter or back exits the application.

I made this just to get an idea for developing for the Flipper Zero, and am only putting it up in a repo, as the guides I had referenced in building this used outdated functions (in particular, mutexes. Some code uses `ValueMutex`, which exists, but is not recommended, some code uses `osMutex` which has been replaced with `FuriMutex`.)

This is meant to be built as a FAP package, which requires a firmware that allows for running applications from the SD card (as of writing, firmware 0.67.2 in the Release category brought this feature.) This also requires knowing how to use the `fbt` utility to build your own package. Refer to the appropriate documentation in the `flipperzero-firmware` repo yourself.

Clone this repo into your `applications_user` directory, and then build it as you see fit with the `fbt` utility.

**THIS IS PROVIDED AS IS AND NO SUPPORT WILL BE PROVIDED**