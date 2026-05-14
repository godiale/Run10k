As user, I want to load web application in my browser.
Application should be written on python.

Application should be represented as a sequence of web pages.
User can click "Prev" and "Next" buttons to navigate.

Each web page should have image "garmin_forerunner.png" from project files as a background picture.
Upper-left corner has coordinates (0, 0) in pixels, down-right corner has coordinates (1536, 1024).
"drawing area" is defined as a rectangle (599, 302) and (930, 567).
Drawing area size is relative to background picture size, both should be changed proportionally.

All banners, text input controls, buttons (including "Prev" and "Next") should fit inside drawing area.
There should be no visible boundary displayed for the drawing area and no background color.
Fonts and lines should be styled as green "monochrome CRT monitor aesthetic".

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
