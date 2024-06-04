The website : https://10-10-91-193.p.thmlabs.com/

Flag 1: THM{HTML_COMMENTS_ARE_DANGEROUS}
How to get here?
The hint is in the comments itself, the problem said that
 
1) What is the flag from the HTML comment?
=> HTML comments are <!-- xyz -->
THIS is how the comments look like.

The comment with 
<!-- This page is temporary while we work on the new homepage @ /new-home-beta -->
/new-home-beta represents a path, which would get that flag, when combined with the complete URL 

Flag 2: THM{NOT_A_SECRET_ANYMORE}

2) What is the directory listing flag?What is the flag from the secret link?
=> Secret Link represents a specific idea, which would apparently be "secret" 
We had to figure out which comment, and the paragraph already made sure to present it as " If you view further down the page source, there is a hidden link to a page starting with "secr", view this link to get another flag. "
Secret link would be another page, and when we scroll down while inspecting the code, we come upto secret-link in <a href="/secret-page">to</a>
So now, we paste this into the url to open up the page https://10-10-91-193.p.thmlabs.com/secret-page

Flag 3: THM{INVALID_DIRECTORY_PERMISSIONS}

3) What is the directory listing flag?
=> " If you view this directory in your web browser, there is a configuration error. What should be displayed is either a blank page or a 403 Forbidden page with an error stating you don't have access to the directory. Instead, the directory listing feature has been enabled, which in fact, lists every file in the directory. Sometimes this isn't an issue, and all the files in the directory are safe to be viewed by the public, but in some instances, backup files, source code or other confidential information could be stored here. In this instance, we get a flag in the flag.txt file. "
These are the lines we need to remember.
As it is mentioned, the files are in the same directoryHow to access it? 
=> https://10-10-91-193.p.thmlabs.com/assets

Flag 4: THM{KEEP_YOUR_SOFTWARE_UPDATED}

4) What is the framework flag?
=> In this scenario, we see the bottom comment:
Page Generated in 0.04856 Seconds using the THM Framework v1.2 ( https://static-labs.tryhackme.cloud/sites/thm-web-framework )
copy the site- https://static-labs.tryhackme.cloud/sites/thm-web-framework
once you reach the page, you'll see the pages 
