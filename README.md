# Notes on these tests #

* Test files are located at http://test.distilled.net/rasmussen/meta2/
* I am debugging them with the [Facebook OG debugger](https://developers.facebook.com/tools/debug/og/object/).

### Tests 1.1 to 1.3 ###
Tests 1.1 to 1.3 began with a stripped-down html page, containing just the socially-relevant tags from the [original page](http://www.rasmussen.edu/career-center/career-research-hub/what-career-is-right-for-me/). Test 1.1 is the original, and then in test 1.2 and 1.3 I turned off suspect  tags(by commenting them out) one by one, testing in https://developers.facebook.com/tools/debug/og/object/ until I found something that worked. I also corrected an issue with some invalid double-quotes.

**What I learned:** As long as og:url and link:canonical are still pointing to the old page and as long as the old page is broken, this page will still be broken.

### Test 1.4 ###
From test 1.4, I reverted to using the original markup, but with the og:url and link:canonical tags removed, and the quote issue fixed as well.

**What I learned:** It still throws issues. There is clearly something else going on with the markup. Test 1.3 works perfectly and Test 1.4 does not, so I just need to find the bit of code in test 1.4 that's throwing errors. 

### Test 1.5 ###
I put test1.4.html through an HTML validator, and began fixing or removing the issues that showed up. **It worked.*

### Test 1.6 ###
I have reverted to test 1.4 and made just a few changes, by removing only the code that looks the most suspect. **It didn't work.**

### Test 1.7 ###
I have reverted to test 1.4 and instead made different changes. **It didn't work either.**

### Test 1.8 ###
Test 1.8 continues from test 1.7 with new changes. **It didn't work either.**

### Test 1.9 ###
Test 1.9 continues from test 8 with new changes. **It works.** So the changes from test 1.8 to test 1.9 are necessary but perhaps not sufficient to fix the problem.

**What I learned:** To fix the issues, make the changes from test7 to test 9, while testing in the OG debugger. When this fixes the problem, begin reverting some of these changes to see if any of them fix it finally.

### Test 2.0 ###
I am continuing from the code in Test 1.9, but working backwards, reintroducing pieces of code one by one. **It broke. Looks like that's one of the issues right there.**

### Test 2.1 ###
Partially reverting the change from 2.0 to see if I can dial in on the problem. **I'm not even sure whether it worked or not: Facebook wasn't very clear, and then it stopped letting me scrape the page because I've been refreshing too many times. :'(**

### Test 2.2 ###
Reverted to the code in Test 1.4, and made only a couple of the changes in test 1.5. **It didn't work** These changes are clearly insufficient.

### Test 2.3 ###
Added more changes on top of the changes the previous test.
**It didn't work** These changes are clearly insufficient.

### Test 2.3 ###
Added more changes on top of the changes the previous test.
**It didn't work** These changes are clearly insufficient.

### Test 2.4 ###
Added more changes on top of the changes the previous test.
**It didn't work** These changes are clearly insufficient.

### Test 2.5 ###
Added more changes on top of the changes the previous test.