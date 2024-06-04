Flag 1: THM{CATCH_ME_IF_YOU_CAN}
Task hint: Many times when viewing javascript files, you'll notice that everything is on one line, which is because it has been minimised, which means all formatting ( tabs, spacing and newlines ) have been removed to make the file smaller. This file is no exception to this, and it has also been obfusticated, which makes it purposely difficult to read, so it can't be copied as easily by other developers. We can return some of the formattings by using the "Pretty Print" option, which looks like two braces { } to make it a little more readable, although due to the obfustication, it's still difficult to comprehend what is going on with the file. If you scroll to the bottom of the flash.min.js file, you'll see the line: flash['remove'](); 
Using pretty print: In firefox, press the bracket option in the bottom, it will turn blue in colour, making it better in readability
Now, see the last few lines, it's line 48.
Click on the line 48, (number)
This adds a breakpoint.
Refresh the page, and you should see the flag
![image](https://github.com/shiroroc/THM---Walking-An-Application/assets/166932167/863b14b2-ba1f-4718-8456-52b0d89e716e)
