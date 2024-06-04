The website : https://10-10-91-193.p.thmlabs.com/

Flag 1: THM{HTML_COMMENTS_ARE_DANGEROUS}
How to get here?
The hint is in the comments itself, the problem said that
 
1) What is the flag from the HTML comment?
=> HTML comments are <!-- xyz -->
THIS is how the comments look like.

The comment with 
<!-- This page is temporary while we work on the new homepage @ /new-home-beta -->
![image](https://github.com/shiroroc/THM---Walking-An-Application/assets/166932167/3963d777-9f8a-48a9-ba12-4cf8a81e1584)

/new-home-beta represents a path, which would get that flag, when combined with the complete URL 
![image](https://github.com/shiroroc/THM---Walking-An-Application/assets/166932167/bab4fe0d-0e86-4d56-a985-dcf1024a74f3)


Flag 2: THM{NOT_A_SECRET_ANYMORE}

2) What is the directory listing flag?What is the flag from the secret link?
=> Secret Link represents a specific idea, which would apparently be "secret" 
We had to figure out which comment, and the paragraph already made sure to present it as " If you view further down the page source, there is a hidden link to a page starting with "secr", view this link to get another flag. "
Secret link would be another page, and when we scroll down while inspecting the code, we come upto secret-link in <a href="/secret-page">to</a>
![image](https://github.com/shiroroc/THM---Walking-An-Application/assets/166932167/e3661978-9db8-432a-b644-85bb05994b2e)

So now, we paste this into the url to open up the page https://10-10-91-193.p.thmlabs.com/secret-page
![image](https://github.com/shiroroc/THM---Walking-An-Application/assets/166932167/83d5b269-b962-4d12-a661-6ca5ed43eeec)


Flag 3: THM{INVALID_DIRECTORY_PERMISSIONS}

3) What is the directory listing flag?
=> " If you view this directory in your web browser, there is a configuration error. What should be displayed is either a blank page or a 403 Forbidden page with an error stating you don't have access to the directory. Instead, the directory listing feature has been enabled, which in fact, lists every file in the directory. Sometimes this isn't an issue, and all the files in the directory are safe to be viewed by the public, but in some instances, backup files, source code or other confidential information could be stored here. In this instance, we get a flag in the flag.txt file. "
These are the lines we need to remember.

As it is mentioned, the files are in the same directory
How to access it? 
=> https://10-10-91-193.p.thmlabs.com/assets
![image](https://github.com/shiroroc/THM---Walking-An-Application/assets/166932167/8118f743-50a3-483d-a7f6-2f0accf0a226)

Flag 4: THM{KEEP_YOUR_SOFTWARE_UPDATED}

4) What is the framework flag?
=> In this scenario, we see the bottom comment:
Page Generated in 0.04856 Seconds using the THM Framework v1.2 ( https://static-labs.tryhackme.cloud/sites/thm-web-framework )
![image](https://github.com/shiroroc/THM---Walking-An-Application/assets/166932167/7ca37c31-c3fd-45cf-b6b5-1c46c205183e)

copy the site- https://static-labs.tryhackme.cloud/sites/thm-web-framework
![image](https://github.com/shiroroc/THM---Walking-An-Application/assets/166932167/30570c8f-ed44-4ee0-be05-4138aa8412cc)

once you reach the page, you'll see the pages: Home • Change Log • Documentation
When we click on change log: ![image](https://github.com/shiroroc/THM---Walking-An-Application/assets/166932167/31f8f68a-e13c-4275-a4f1-32d414a977d9)
and download tmp.zip
but, when we try to use https://static-labs.tryhackme.cloud/sites/thm-web-framework/changelog.html, it does not return the answer.
Now read the paragraph again, it is said that it was moved to a place unreadable by website visitors.
Meaning, some other place, which in this case would be simply the previous site https://10-10-91-193.p.thmlabs.com/tmp.zip
Download it, and you have the last flag

