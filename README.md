# An Experimental Webring Implementation

## How it works.

A list of sites in the webring is contained in the json file, website using the ring can pull the list of sites using fetch within their javascript.

An seperate webpage holding all of the sites and some stylization for the ring is also in the repo, sites can also link to this page for users to navigate the whole ring.

Ideally websites would be able to find where they are in the json as well as their nearest neighbors for next and last buttons.
