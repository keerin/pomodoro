# Pomodoro
## A very simple command-line countdown timer

This is most likely a perpetual work in progress, so apologies if you have to jump through hoops to get this to run.

I use Ruby 2.2.1, but as far as I know, everything here works with every version of Ruby.

You will have to install mpg123 to make the beep work at the end. If you find it does not work, just change:
    `mpg123 -q ~/Documents/projects/pomodoro/beep.mp3`
to
    print "\a"

The terminal bell doesn't work on my machine for unknown reasons, and it doesn''t annoy me enough to spend half the day messing about trying to get it to work. If you want the timer to use mpg123 if it exists, or print "\a" if it does not then feel free to respond to an issue and pull.

### Useage

    $ pomodoro -t 20

Will run the timer in the terminal for 20 minute, counting down in seconds.

    $ pomodoro -t 1

Will run the timer in the terminal for 1 minutes, counting down in seconds.

That's it so far.

### To Do

1. Add help flags and documentation
2. Use terminal bell if user does not have mpg123 installed
3. Allow the user to also enter a time containing seconds (5.5 = 5 min 30 secs)
4. Allow the user to display countdown in seconds or minutes and seconds
