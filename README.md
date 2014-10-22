# Notes on these tests #

### Tests 1 to 3 ###
Tests 1 to 3 began with a stripped-down html page, containing just the socially-relevant tags from the [original page](http://www.rasmussen.edu/career-center/career-research-hub/what-career-is-right-for-me/). Test 1 is the original, and then in test 2 and 3 I turned off suspect  tags(by commenting them out) one by one, testing in https://developers.facebook.com/tools/debug/og/object/ until I found something that worked. I also corrected an issue with some invalid double-quotes.
** What I learned is that as long as og:url and link:canonical are still pointing to the old page and as long as the old page is broken, this page will still be broken. **

### Test 4 ###
From test 4, I reverted to using the original markup, but with the og:url and link:canonical tags removed, and the quote issue fixed as well.
** What I learned: It still throws issues. There is clearly something else going on with the markup. Test 3 works perfectly and Test 4 does not, so I just need to find the bit of code in test 4 that's throwing errors. ** 

### Test 5 ###
I put test4.html through an HTML validator, and began fixing or removing the issues that showed up.

### Test 6 ###
ok so test5 worked. I have reverted to test5 and made just a few changes, by removing only the code that looks the most suspect.

### Test 7 ###
Test 6 didn't work: It still broke. I have reverted test 6 and instead made different changes.

### Test 8 ###
Test 7 didn't work either. Test 8 continues from test 7 with new changes.

### Test 9 ###
Test 8 didn't work either. Test 9 continues from test 8 with new changes.