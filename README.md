# An enhanced Actor Framework Message Maker!

Key improvements over NI's Actor Framework Message Maker:

* Ability to update already built messages
* New message icons
* Send Message VI gets its description from the message VI


To use the tool open a your project then select "Tools"->"LSI Actor Framework Message Maker". Next select the methods you'd like to create messages for and click "Build/Update Selected Messages"

The actor framework message maker supplied by NI has two important limitations:
1. If you changed the message VI, you had to manually fix the message class
2. A lot of block diagram readability is lost because of the plain "Send Message" VIs, and it takes a lot of time to go in and change the icons and descriptions.

This new message maker aims to fix both of these issues. 

First, you can update messages. The message maker automatically detects which messages are out of date, and the user just has to click a button. 

Next, readability. There were two main things that a message needed to significantly increase block diagram readability. First, it needs a good icon. The icon should clearly show that it's a message, but also tell you what the message does. To do this, we steal parts of the icon from your source code to create a distinct and helpful icon. Second, it needs a good VI description. This is again stolen from the message VI. Now you can look at a block diagram, mouse over things, and get a good idea of what your actor code is doing.