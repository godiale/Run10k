As user, I want to load web application in my browser.
Application should be written on python.

Application should be represented as a sequence of web pages.
User can click "Prev" and "Next" buttons to navigate.

Use "garmin_forerunner.jpg" from project files as a background picture on each page.
This picture contains image of watches with round black display. 
Draw all web controls inside watches' display, using green "monochrome CRT monitor aesthetic" shrift.

On the first page, application shows banner "Herzlich Willkommen!".

On the second page, application shows:
* Banner "Enter Garmin Connect credentials"
* Text field "Username" and input field to get username.
* Text field "Password" and input field to get password.
* A button "Connect..."

Upn clicking the button, application should authenticate to Garmin Connect API with entered credentials.
* If username and password are correct - popup "Connection successful" is shown. Application moves to next page.
* If username or password are incorrect - popup "Username or Password is incorrect" is shown. Application stays on current page.

Once connection is successful, second page is not shown in current browser session.
Application should hold Garmin Connect API session and use it to get data.

On the third page application shows following information.
* How many days starting 07.08.2020 I had at least 1 running training (running days done). Call it "Running days".
* Calculate average runs rate per day from the history, predict and display the date, when I reach 10000 running days, with this rate. Call it "Estimated completion".
