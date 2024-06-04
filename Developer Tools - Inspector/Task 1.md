Flag 1: THM{NOT_SO_HIDDEN}

1)What is the flag behind the paywall?
Steps to follow: Locate the DIV element with the class premium-customer-blocker and click on it. You'll see all the CSS styles in the styles box that apply to this element, such as margin-top: 60px and text-align: center. The style we're interested in is the display: block. If you click on the word block, you can type a value of your own choice. Try typing none, and this will make the box disappear, revealing the content underneath it and a flag. If the element didn't have a display field, you could click below the last style and add in your own. Have a play with the element inspector, and you'll see you can change any of the information on the website, including the content. Remember this is only edited on your browser window, and when you press refresh, everything will be back to normal.

![image](https://github.com/shiroroc/THM---Walking-An-Application/assets/166932167/34e42c78-5fa3-4400-bcfa-2f49b48d0f54)
now, replace it with none:
![image](https://github.com/shiroroc/THM---Walking-An-Application/assets/166932167/c6da14ff-6ebe-4faf-96f3-85b28622aa30)

