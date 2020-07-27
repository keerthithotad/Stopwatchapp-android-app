# Stopwatchapp-android-app
The Stopwatch app consists of a single activity and a single layout.The layout includes a text view showing you how much time haspassed, a Start button that starts the stopwatch, a Stop button thatstops it, and a Reset button that resets the timer value to 0.
# Create a new project for the Stopwatch app
# Add String resources.
# Update the stopwatch layout code.
# How the activity code will work
The layout defines three buttons that we’ll use to controlthe stopwatch. Each button uses its onClick attributeto specify which method in the activity should run whenthe button is clicked. When the Start button is clicked, theonClickStart() method gets called, when the Stopbutton is clicked the onClickStop() method gets called,and when the Reset button is clicked the onClickReset()method gets called. We’ll use these methods to start, stop, andreset the stopwatch.
# Add code for the buttons.
When the user clicks on the Start button, we’ll set the running variable to true so that the stopwatch will start. When the user clicks on the Stop button, we’ll set running to false so that the stopwatch stops running. If the user clicks on the Reset button, we’ll set running to false and seconds to 0 so that the stopwatch is reset and stops running.
# What happens when you run the app?
1)The user decides to wants run the app.
2)An intent is constructed to start this activity using startActivity(intent).
3)Android checks to see whether there’s already a process running for the app, and if not, creates a new process. 
4)The onCreate() method in the activity gets called. 
The method includes a call to setContentView(), specifying a layout, and then starts the stopwatch with runTimer().
5)When the onCreate() method finishes, the layout gets displayed on the device.
The runTimer() method uses the seconds variable to determine what text to display in the text view, and uses the running variable to determine whether to increment the number of seconds. As running is initially false, the number of seconds isn’t incremented.
6)Test drive the app.
7)Rotating the screen changes the device configuration.
8)The user rotates the device.
9)Android destroys the activity, and then recreates it. 
10)The Bundle contains the values of the seconds and running variables as they were before the activity was destroyed.
11)The runTimer() method gets called, and the timer picks up where it left off.
