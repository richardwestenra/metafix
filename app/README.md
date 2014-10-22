# Notes on this test #

### Tests 1 to 3 ###
Tests 1 to 3 began with a stripped-down html page, containing just the socially-relevant tags from the [original page](http://www.rasmussen.edu/career-center/career-research-hub/what-career-is-right-for-me/). Test 1 is the original, and then in test 2 and 3 I turned off suspect  tags(by commenting them out) one by one, testing in https://developers.facebook.com/tools/debug/og/object/ until I found something that worked. I also corrected an issue with some invalid double-quotes.
** What I learned is that as long as og:url and link:canonical are still pointing to the old page and as long as the old page is broken, this page will still be broken. **

### Test 4 ###
From test 4, I reverted to using the original markup, but with the og:url and link:canonical tags removed, and the quote issue fixed as well.