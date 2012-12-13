# Coursera as a Podcast

This is a tiny project that was only done to ease access to Coursera content from iOS devices. The Coursera 
website isn't the most compelling site to use from a mobile device, so I created a podcast feed generator by scraping
their website and parsing relevant URLs and descriptions.

The `courses.json` file in the root folder is the list of course URLs from which the generator will generate feeds 
(and place them in the `feeds/` subfolder). You can call the generator from the terminal :

    $ ./generate
    
On my MacBook Pro, it takes about 40 seconds to fetch and generate feeds for all courses.

And, yeah, it works without credentials or any form of authentication.
