# Answers-to-Chapter-11
Ch11_Answers
1. Brieﬂy describe the differences between the webbrowser, requests, BeautifulSoup, and selenium modules.
Answer: 1. The webbrowser module has an open() method that will launch a web browser to a speciﬁc URL, and that’s it. The requests module can download ﬁles and pages from the Web. The BeautifulSoup module parses HTML. Finally, the selenium module can launch and control a browser. 
2. What type of object is returned by requests.get()? How can you access the downloaded content as a string value?
Answer: 2. The requests.get() function returns a Response object, which has a text attribute that contains the downloaded content as a string. 
3. What Requests method checks that the download worked?
Answer: 3. The raise_for_status() method raises an exception if the download had problems and does nothing if the download succeeded. 
4. How can you get the HTTP status code of a Requests response?
Answer: 4. The status_code attribute of the Response object contains the HTTP  status code. 
5. How do you save a Requests response to a ﬁle?
Answer: 5. After opening the new ﬁle on your computer in 'wb' “write binary” mode, use a for loop that iterates over the Response object’s iter_content() method to write out chunks to the ﬁle. Here’s an example:
saveFile = open('filename.html', 'wb') for chunk in res.iter_content(100000):    saveFile.write(chunk)
6. What is the keyboard shortcut for opening a browser’s developer tools?
Answer:  6. F12 brings up the developer tools in Chrome. Pressing CTRL-SHIFT-C (on Windows and Linux) or z-OPTION-C (on OS X) brings up the developer tools in Firefox. 
7. How can you view (in the developer tools) the HTML of a speciﬁc element on a web page?
Answer: 7. Right-click the element in the page, and select Inspect Element from the menu. 
8. What is the CSS selector string that would ﬁnd the element with an id attribute of main?
Answer: 8. '#main' 
9. What is the CSS selector string that would ﬁnd the elements with a CSS class of highlight?
Answer: 9. '.highlight' 
10. What is the CSS selector string that would ﬁnd all the <div> elements inside another <div> element?
Answer: 10. 'div div' 
11. What is the CSS selector string that would ﬁnd the <button> element with a value attribute set to favorite?
Answer: 11. 'button[value="favorite"]' 
12. Say you have a Beautiful Soup Tag object stored in the variable spam for the element <div>Hello world!</div>. How could you get a string 'Hello world!' from the Tag object?
Answer: 12. spam.getText() 
13. How would you store all the attributes of a Beautiful Soup Tag object in a variable named linkElem?
Answer: 13. linkElem.attrs 
14. Running import selenium doesn’t work. How do you properly import the selenium module?
Answer: 14. The selenium module is imported with from selenium 
import webdriver. 
15. What’s the difference between the find_element_* and find_elements_* methods?
Answer: 15. The find_element_* methods return the ﬁrst matching element as a WebElement object. The find_elements_* methods return a list of all  matching elements as WebElement objects. 
16. What methods do Selenium’s WebElement objects have for simulating mouse clicks and keyboard keys?
Answer: 16. The click() and send_keys() methods simulate mouse clicks and keyboard keys, respectively. 
17. You could call send_keys(Keys.ENTER) on the Submit button’s WebElement object, but what is an easier way to submit a form with Selenium?
Answer: 17. Calling the submit() method on any element within a form submits the form. 
18. How can you simulate clicking a browser’s Forward, Back, and Refresh buttons with Selenium?
Answer: 18. The forward(), back(), and refresh() WebDriver object methods simulate these browser buttons. 

