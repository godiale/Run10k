As user, I want to load web application in my browser.
Application should be written on python.

Application should be represented as a sequence of web pages.
User can click "Prev" and "Next" buttons to navigate.

Each web page should have image "garmin_forerunner.png" from project files as a background picture.
This picture contains image of watches with round black display, having circle shape.
Analyze the picture, find black circle shape area, determine its position and size. Lets name it "drawing area".
All banners, text input controls, buttons that application shows to the user, should fit inside "drawing area" and styled as green "monochrome CRT monitor aesthetic".

On the first page, application shows banner "Herzlich Willkommen!".

On the second page, application shows:
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
