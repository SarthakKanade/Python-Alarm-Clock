This Python script implements an alarm clock application with a graphical user interface (GUI) using Tkinter. The application includes features such as setting multiple alarms with custom sounds, playing motivational quotes, and snoozing alarms. The code also uses Pygame for playing sound files.

Description of the Code:
Imports:

The script imports necessary modules including time, datetime, pygame, random, threading, and tkinter.
pygame.mixer.init() initializes the Pygame mixer for playing sounds.
Motivational Quotes:

A list of motivational quotes is defined to be displayed when the user chooses to play a quote.
Alarms Dictionary:

An empty dictionary alarms is used to store alarm times and their corresponding sound files.
Functions:

play_sound(sound_file): Plays the specified sound file using Pygame.
play_quote(): Displays a random motivational quote in a message box.
set_alarm(time_str, sound_file): Adds an alarm to the alarms dictionary with the specified time and sound file.
check_alarms(): Continuously checks the current time against the set alarms and plays the corresponding sound if an alarm is due. This function runs in a separate thread to allow continuous checking without blocking the main program.
Tkinter GUI:

The GUI components and layout are defined using Tkinter. This includes input fields for setting alarm times, buttons for setting alarms, snoozing, and playing quotes, and a canvas for displaying a round clock face with dynamically updating hands.
The script is designed to provide a user-friendly interface for setting and managing alarms, with additional features to enhance the waking-up experience through motivational quotes and custom sounds.
