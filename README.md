# 🍅Pomodoro Timer App using Tkinter of Python

🌟A GUI intergrated Pomodoro Timer App which helps you track your Work sessions & Break sessions.

🌟In Pomodoro technique the Work session are defined for 25 minutes and the break session are defined for 5 minutes. 
After four successful work sessions a long break of 20 minutes is awarded.

👉The UI setup of the app is done using the tkinter classes like Label, Button, Tk, PhotoImage and Canvas.

👉The Canvas class is used to design the background of the app and also to add the image and the timer countdown text.

👉The countdown mechanism is programmed using the 'window.after(...)' method which updates the window every second and its
functioning is implemented by using a recursive function call of the 'count_down' function.

👉A variable 'reps' is used to track the number of successful work sessions for the timer value to update and the checkmark to display.

👉The app begins with the pressing of the 'Start' button which has a command start_timer tied to it. The button press calls the function 'start_timer' 
which first converts the timings in minutes into their seconds equivalent. 

👉The 'start_timer' then, based on the number of reps completed allocates the respective amount of time and calls the 'count_down' function 
passing the appropriate time as its argument.

👉The 'count_down' function takes in, time in seconds as a argument and then converts it into minutes and seconds left using appropriate 
logic. This updated time is used to change the timer text on the app window. Also, the number of reps successfully completed is displayed to user updating the 
checkmark label.

👉The app timer is reset by clicking the 'reset' button which calls the 'reset_timer' funtion. 

👉The 'reset_timer' function uses the method 'window.after_cancel(...)' to stop the timer and stop the window updation per second. It is here only that
the various objects, labels and texts are updated and reset to their initial values.

![App Start window](https://github.com/bellaryyash23/pomodoro_tkinter/blob/master/start.JPG?raw=true)

App Starting window 👆 

![Work session window](https://github.com/bellaryyash23/pomodoro_tkinter/blob/master/work.JPG?raw=true)

App Work Session window👆

![Break session window](https://github.com/bellaryyash23/pomodoro_tkinter/blob/master/break.JPG?raw=true)

App Break Session window👆
