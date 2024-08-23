# An Experimental Webring Implementation

## How it works.

A list of sites in the webring is contained in the json file, website using the ring can pull the list of sites using fetch within their javascript.

An seperate webpage holding all of the sites and some stylization for the ring is also in the repo, sites can also link to this page for users to navigate the whole ring.

Ideally websites would be able to find where they are in the json as well as their nearest neighbors for next and last buttons.

### How the JSON Works
The json file is a nx4 array of websites which ring members will refference.

Each entry has four data points.
Name: The Name of the website intended to be read by humans.

Address: The URL of the website.

nextOveride: Specifies if a website prefers for its next button to go to a specific website. If set to none, the website will navigate to the entries immediately before and after itself.

prevOveride: Same as nextOveride but backwards.

### How the webring decides who's next.
