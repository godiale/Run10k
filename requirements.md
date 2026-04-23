As user, I want to load web application in my browser.
It should consist of sequence of Web pages.

Application should be written on python.

All Web pages background should be styled as below:
* Clear blue sky with the sun shining in the left upper corner
* In the right upper corner -- big slogan "Project Run10k"
* In the center -- big Garmin Forerunner 230 (black) watches, more than 80% of area of the screen.
* All further controls should be drawn inside this Forerunner screen (like in the frame)

On the first page I see following controls:
* Invitation to enter Garmin Connect credentials
* Garmin Connect username entry.
* Garmin Connect password entry.
* A button "Connect"

As user, I can entry my Garmin Connect username and password and press "Connect".
Application then connects to my Garmin Connect account data via API
* If username and password are correct -- it can read my trainings history.
* If username or password are not correct -- application returns to the first screen,
  and show small banner to me as a user, that credentials are not correct.

After successful reading data from my Garmin Connect account, program displays second page.

On the second page I as a user see following information:
* How many days starting 07.08.2020 I had at least 1 running training (running days done).
* How many days remaining till 10000 days with runs (10000 - number of runnings days done).
* Calculate average runs rate per day from the history, predict and display the date, when I reach 10000 running days, with this rate.


