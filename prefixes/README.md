## Introduction

Long, long ago on an enshittified internet forum, I proposed the idea of a registry for unique id prefixes. I was having a bit of difficulty naming ebook files, as not all notable books have ISBN numbers. Scans of older works, ebooks published by organizations that can't afford to purchase ISBNs or choose not to do so, etc. There exist multiple alternatives to ISBNs, of course, but none are universal and in any case their identification numbers/strings are predictably very similar so who can tell if that's a Library of Congress number or an OCLC number or a Gutenberg Project catalog number? Thus, the idea of having a short, standard prefix that you could prepend to these was born.

This repo will (in part) act as a registry for any such prefixes. Submit pull requests and issues as necessary.

## Guidelines for a unique id prefix proposal:

1. Each should consist of 3-4 ascii/latin alphabetic letters.
2. These are not case sensitive, but in the list please use uppercase for visual purposes.
3. Please include a link to the relevant company, institution, or failing that, a wikipedia link that can help explain your usage.
4. This is free, and unmanaged. There should be no cause for name-squatting. If you believe that a prefix has been used incorrectly, please open an issue.

## Usage

Usage will vary from file type to file type. The prefix should be uppercase and prepended to the number/string, with a unicode bullet character `•` as the separator. 

### Books
Best practice is to include the unique ID within the filename itself. ISBN-13 is the preferred identifier, followed by LCCN and OCLC (whichever is available). ISBN-10 numbers can be converted to ISBN-13 with various online tools. All spaces and dashes should be removed for the number for filename length considerations. ISBN-13 numbers always begin with `978-` and the prefix is optional, all others should be prepended with the four character code.

### Magazines / journals / comic books
ISSN is the preferred identifier. If the nature of the files makes it clear that this is a serial work (magazine, journal, etc.), the ISSN prefix is optional. OCLC can serve as a fallback for historical serials that were never issued ISSNs. Best practice is to include the ISSN or OCLC number in the parent folder name in parentheses, e.g.: 

    Australian Woodsmith (1441-0311)/
    Hollywood Reporter, The (0018-3660)/
    Lubbock Avalanche-Journal (OCLC•13942131)/
    Piecework (2377-7591)

For duplicate nationalized titles (most popular magazines like Rolling Stone, Reader's Digest, etc.), additional disambiguation can be included within the parentheses separated by commas:

    Playboy (0156-8892, au)
    Vogue (0262-2130, uk)

### Other file types
Use best judgement. File naming conventions are often dictated by software systems such as Plex, which are relatively inflexible in the matter of filenames.

## Prefixes

### Books / Literature / Written works
* `4CHN` - $${\color{red}NSFW}$$ [4chan](https://4chan.org/) -
* `ASIN` - [Amazon](https://www.amazon.com/) - 
* `AOOO` - [Archive of Our Own](https://archiveofourown.org/) - 
* `ASTR` - $${\color{red}NSFW}$$ [ASSTR](https://asstr.org/) -
* `ARXV` - [arXiv](https://arxiv.org/) -
* `BXIV` - [Beilstein Archives](https://www.beilstein-archives.org/xiv/) - 
* `DPCA` - [Distributed Proofreaders of Canada](https://www.pgdpcanada.net/) - 
* `FADE` - [Faded Page](https://www.fadedpage.com/) - 
* `FANF` - [Fanfiction.net](https://www.fanfiction.net/) -
* `GTNA` - [Project Gutenberg Australia](https://gutenberg.net.au/) - 
* `GTNB` - [Project Gutenberg](https://www.gutenberg.org/) - 
* `GTNC` - [Project Gutenberg Canada](https://gutenberg.ca/) - 
* `ISBN` - [International Standard Book Number](http://www.isbn.org/) - [&lt;ID format&gt;](https://en.wikipedia.org/wiki/ISBN#Overview)
* `ISMN` - [International Standard Music Number](https://www.ismn-international.org/) - 
* `ISSN` - [International Standard Serial Number](https://www.issn.org/) (periodicals) -
* `ISFD` - [Internet Speculative Fiction Database](https://www.isfdb.org) (series) - 
* `MRXV` - [medRxiv](https://www.medrxiv.org/) - 
* `MUSE` - [Musescore](https://musescore.com/) - 
* `LCCN` - [Library of Congress Control Number](https://en.wikipedia.org/wiki/Library_of_Congress_Control_Number) -
* `LIVJ` - [Livejournal](https://www.livejournal.com/) -
* `OCLC` - [OCLC](https://en.wikipedia.org/wiki/OCLC#Identifiers_and_linked_data) -
* `OLIB` - [Open Library](https://openlibrary.org/) - 
* `REDD` - [Reddit](https://old.reddit.com/) - 
* `SCPF` - [SCP Foundation](https://scp-wiki.wikidot.com/) -
* `SEPH` - [Stanford Encyclopedia of Philosophy](https://plato.stanford.edu/) - 
* `TUMB` - [Tumblr](https://www.tumblr.com/) -
* `VIXA` - [viXra](https://vixra.org/) - 
* `WIKI` - [Wikipedia](https://en.wikipedia.org/wiki/Main_Page) -
* `WORP` - [Wordpress](https://wordpress.com/) -

### Video / Films / Shows
* `DMOT` - [Daily Motion](https://dailymotion.com/) - 
* `VIME` - [Vimeo](https://vimeo.com/) - 
* `YOUT` - [YouTube](https://youtube.com/) - [&lt;ID format&gt;](formats/yout.md)

### Art
* `DEVA` - [Deviant Art](https://www.deviantart.com/)

### Recipes
* `ALLR` - [Allrecipes.com](https://www.allrecipes.com/)
* `ALTO` - []()
* `BETC` - []()
* `EATW` - [Eatingwell.com](https://www.eatingwell.com/)
* `EPIC` - [Epicurious.com]()
* `FDNT` - [Foodnetwork.com]
* `FOOD` - [Food.com]()
* `YUMM` - [Yummly.com]()

### Humans
* `ISNI` - [International Standard Name Identifier](https://en.wikipedia.org/wiki/International_Standard_Name_Identifier) - <format as issued by that org>
* `ORCI` - [ORCID](https://en.wikipedia.org/wiki/ORCID) - 

### Langauges
* `ETHN` - [Ethnologue](https://www.ethnologue.com/) - 
* `GLOT` - [Glottolog](https://glottolog.org/) -
* `ISOL` - [ISO 639](https://en.wikipedia.org/wiki/List_of_ISO_639_language_codes) -
* `LING` - [Linguasphere Observatory](https://linguasphere.info/) -

### Plans / blueprints / physibles
* `THNG` - [Thingiverse](https://www.thingiverse.com)

### Garment patterns
* `BURD` - [Burda Style](https://simplicity.com/) - 
* `BTRK` - [Butterick](https://simplicity.com/) -
* `KNOW` - [Know Me](https://simplicity.com/) -
* `MCCA` - [McCall's](https://simplicity.com/) -
* `NWLK` - [New Look](https://simplicity.com/) -
* `SIMP` - [Simplicity](https://simplicity.com/) -
* `THTH` - [Thread Theory](https://threadtheory.ca/) -
* `VOPA` - [Vogue Patterns](https://simplicity.com/) -
