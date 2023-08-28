# google_like_a_PRO

# Google like a PRO

## Content


[Search Operators by word](#search-operators-by-word)

[Logical Search Operators and range](#logical-search-operators-and-range)

[Search type operators](#search-type-operators)

[DNS search operators](#dns-search-operators)

[Data search operators](#data-search-operators)

[Find indexation errors](#find-indexation-errors)

[Find non-secure pages (non-https)](#find-non-secure-pages-non-https)

[Find duplicate content issues](#find-duplicate-content-issues)

[Find odd files on your domain (that you may have forgotten about)](#find-odd-files-on-your-domain-that-you-may-have-forgotten-about)

[Find guest post opportunities](#find-guest-post-opportunities)

[Find social profiles for outreach prospects](#find-social-profiles-for-outreach-prospects)


## Search Operators by word

### "search term"

Force an exact-match search. Use this to refine results for ambiguous searches, or to exclude synonyms when searching for single words.

```txt
"steve jobs"
```

### *

Acts as a wildcard and will match any word or phrase.
Example:
```txt
steve * apple
```

### $

Search for prices. Also works for Euro (€), but not GBP (£)
Example:
```txt
ipad $329
```

### define:

A dictionary built into Google, basically. This will display the meaning of a word in a card-like result in the SERPs.
Example:
```txt
define:entrepreneur
```

### intitle:

Find pages with a certain word (or words) in the title. In our example, any results containing the word “apple” in the title tag will be returned.
Example:
```txt
intitle:apple
```

### allintitle:

Similar to “intitle,” but only results containing all of the specified words in the title tag will be returned.
Example:
```txt
allintitle:apple iphone
```

### intext:

Find pages containing a certain word (or words) somewhere in the content. For this example, any results containing the word “apple” in the page content will be returned.
Example:
```txt
intext:apple
```

### allintext:

Similar to “intext,” but only results containing all of the specified words somewhere on the page will be returned.
Example:
```txt
allintext:apple iphone
```

### _

Not exactly a search operator, but acts as a wildcard for Google Autocomplete.
Example: 
```txt
apple CEO _ jobs
```

### +

Force an exact-match search on a single word or phrase.
Example:
```txt
jobs +apple
```

### ~

Include synonyms. Doesn’t work, because Google now includes synonyms by default. (Hint: Use double quotes to exclude synonyms.)
Example:
```txt
~apple
```

[Content](#content)

## Logical Search Operators and range

### OR

Search for X or Y. This will return results related to X or Y, or both. Note: The pipe (|) operator can also be used in place of “OR.”
Examples:
```txt
jobs OR gates 
```
```txt
jobs | gates
```

### AND

Search for X and Y. This will return only results related to both X and Y. Note: It doesn’t really make much difference for regular searches, as Google defaults to “AND” anyway. But it’s very useful when paired with other operators.
Example:
```txt
jobs AND gates
```

### -

Exclude a term or phrase. In our example, any pages returned will be related to jobs but not Apple (the company).
Example:
```txt
jobs -apple
```

### ( )

Group multiple terms or search operators to control how the search is executed.
Example:
```txt
(ipad OR iphone) apple
```

### AROUND(X)

Proximity search. Find pages containing two words or phrases within X words of each other. For this example, the words “apple” and “iphone” must be present in the content and no further than four words apart.
Example:
```txt
apple AROUND(4) iphone
```

### #..#

Search for a range of numbers. In the example below, searches related to “WWDC videos” are returned for the years 2010-2014, but not for 2015 and beyond.
Example:
```txt
wwdc video 2010..2014
```

[Content](#content)

## Search type operators

### cache:

Returns the most recent cached version of a web page (providing the page is indexed, of course).
Example:
```txt
cache:apple.com
```

### filetype:

Restrict results to those of a certain filetype. E.g., PDF, DOCX, TXT, PPT, etc. Note: The “ext:” operator can also be used—the results are identical.
Example:
```txt
apple filetype:pdf
```
```txt
apple ext:pdf
```

### weather:

Find the weather for a specific location. This is displayed in a weather snippet, but it also returns results from other “weather” websites.
Example:
```txt
weather:san francisco
```

### stocks:

See stock information (i.e., price, etc.) for a specific ticker.
Example:
```txt
stocks:aapl
```

### map:

Force Google to show map results for a locational search.
Example:
```txt
map:silicon valley
```

### movie:

Find information about a specific movie. Also finds movie showtimes if the movie is currently showing near you.
Example:
```txt
movie:steve jobs
```

### in

Convert one unit to another. Works with currencies, weights, temperatures, etc.
Example:
```txt
$329 in GBP
```

### source:

Find news results from a certain source in Google News.
Example:
```txt
apple source:the_verge
```

### loc:placename

Find results from a given area.
Example:
```txt
loc:"san francisco" apple
```

### inpostauthor:

Find blog posts written by a specific author. This only worked in Google Blog search, not regular Google search.
Example: 
```txt
inpostauthor:"steve jobs"
```

### allinpostauthor:

Similar to “inpostauthor,” but removes the need for quotes (if you want to search for a specific author, including surname.)
Example: 
```txt
allinpostauthor:steve jobs
```

### inposttitle:

Find blog posts with specific words in the title. No longer works, as this operator was unique to the discontinued Google blog search.
Example: 
```txt
intitle:apple iphone
```

### info:

Find information about a specific page, including the most recent cache, similar pages, etc. (Deprecated in 2017). Note: The id: operator can also be used—the results are identical.
Example:
```txt
info:apple.com
```
```txt
id:apple.com
```

### phonebook:

Find someone’s phone number. (Deprecated in 2010)
Example:
```txt
phonebook:tim cook
```

### #

Searches #hashtags. Introduced for Google+; now deprecated.
Example:
```txt
#apple
```

[Content](#content)

## DNS search operators

### site:

Limit results to those from a specific website.
Example:
```txt
site:apple.com
```

### related:

Find sites related to a given domain.
Example:
```txt
related:apple.com
```

### inurl:

Find pages with a certain word (or words) in the URL. For this example, any results containing the word “apple” in the URL will be returned.
Example:
```txt
inurl:apple
```

### allinurl:

Similar to “inurl,” but only results containing all of the specified words in the URL will be returned.
Example:
```txt
allinurl:apple iphone
```


### inanchor:

Find pages that are being linked to with specific anchor text. For this example, any results with inbound links containing either “apple” or “iphone” in the anchor text will be returned.
Example:
```txt
inanchor:apple iphone
```

### allinanchor:

Similar to “inanchor,” but only results containing all of the specified words in the inbound anchor text will be returned.
Example:
```txt
allinanchor:apple iphone
```

### blogurl:

Find blog URLs under a specific domain. This was used in Google blog search, but I’ve found it does return some results in regular search.
Example:
```txt
blogurl:microsoft.com
```

### link:

Find pages linking to a specific domain or URL. Google killed this operator in 2017, but it does still show some results—they likely aren’t particularly accurate though. (Deprecated in 2017)
Example:
```txt
link:apple.com
```

[Content](#content)

## Data search operators


### before:	

Search for results from before a particular date.	
```txt
apple before:2007-06-29
```

### after:	

Search for results from after a particular date.	
```txt
apple after:2007-06-29
```

### daterange:

Find results from a certain date range. Uses the Julian date format, for some reason.
Example:
```txt
daterange:11278-13278
```

[Content](#content)


## Find indexation errors

```txt
site:ahrefs.com

site:ahrefs.com/blog

site:*.ahrefs.com -www

```
wildcard (*) operator to find all subdomains belonging to the domain, combined with the exclusion operator (-) to exclude regular www results

`site:yourblog.com/category`- find WordPress blog category pages;

`site:yourblog.com inurl:tag` -  find WordPress “tag” pages

[Content](#content)

## Find non-secure pages (non-https)

```txt
site:asos.com -inurl:https

```

[Content](#content)

## Find duplicate content issues

```txt
site:asos.com"The modern Abercrombie & Fitch is the next"

- site:asos.com"The modern Abercrombie & Fitch is the next"

site:asos.com"* Abercrombie & Fitch is the next"

```

[Content](#content)

## Find odd files on your domain (that you may have forgotten about)

```txt
site:ahrefs.com filetype:pdf

site:ahrefs.com (ext:PDF OR ext:docx OR ext:txt OR ext:ppt OR ext:xls)

```

[Content](#content)

## Find guest post opportunities

```txt
fitness intitle:"write for us" inurl:"write-for-us"

"become a contributor"

"contribute to"

"write for me"

"guest post guidelines"

inurl:guest-post

inurl:guest-contributor-guidelines

fitness ("write for us" | inurl:"guest-post-guidelines" | inurl:"guest-post")

(fitness | health) AND ("write for us" | inurl:"guest-post-guidelines")

(fitness | health) AND ("write for us" | inurl:"guest-post-guidelines") AND site:.co.uk
```

[Content](#content)

## Find social profiles for outreach prospects

```txt
steve jobs apple (site:twittert.com | site:facebook.com | site:linkedin.com)

"become a contributor"

"contribute to"

"write for me"

"guest post guidelines"

inurl:guest-post

inurl:guest-contributor-guidelines

fitness ("write for us" | inurl:"guest-post-guidelines" | inurl:"guest-post")

(fitness | health) AND ("write for us" | inurl:"guest-post-guidelines")

(fitness | health) AND ("write for us" | inurl:"guest-post-guidelines") AND site:.co.uk
```

[Article](https://www.thenextseo.co.in/google-search-operators-the-complete-list/35715)

[Content](#content)
