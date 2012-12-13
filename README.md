# Coursera as a Podcast

This is a tiny project that was only done to ease access to Coursera content from iOS devices. The Coursera 
website isn't the most compelling site to use from a mobile device, so I created a podcast feed generator by scraping
their website and parsing relevant URLs and descriptions.

The `courses.json` file in the root folder is the list of course URLs from which the generator will generate feeds 
(and place them in the `feeds/` subfolder). You can call the generator from the terminal (given you have node and coffee-script installed) :

    $ ./generate
    
On my MacBook Pro, it takes about 40 seconds to fetch and generate feeds for all courses.

And, yeah, it works without credentials or any form of authentication.

## Prerequisites

For it to work, you need to have node and coffee-script installed and their executable accessible. If you don't, and you're on a Mac (of course you are)

    $ brew install node
    $ npm i -g coffee-script

Then, in this project's root folder:

    $ npm i jsdom jstoxml underscore.string


