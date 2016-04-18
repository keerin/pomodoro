# Pomodoro
## A very simple command-line countdown timer

This is most likely a perpetual work in progress, so apologies if you have to jump through hoops to get this to run.

I use Ruby 2.2.1, but as far as I know, everything here works with every version of Ruby.

The terminal bell doesn't work on my machine for unknown reasons, and it doesn't annoy me enough to spend half the day messing about trying to get it to work. This is the only reason for the -m switch. Using terminal bell is the defaut because I imagine my problem is an edge case.

### Usage

Simply type 'pomodoro' into the command line, and you'll be given a 20 minute timer. Hit CTRL+C to terminate.

    $ pomodoro

Will run the countdown timer for 20 minutes, counting down in minutes and seconds, and will emit a system beep when finished.

    $ pomodoro -t 15

Will run the timer in the terminal for 15 minutes, counting down in minutes and seconds, and will emit a system beep when finished.

    $ pomodoro -m -t 1

Will run the timer in the terminal for 1 minutes, counting down in minutes and seconds, and will try to use mpg123 to play beep.mp3 when finished.

    $ pomodoro --mpg
    
Will run the countdown timer for 20 minutes, counting down in minutes and seconds, and will try to use mpg123 to play beep.mp3 when finished.

    $ pomodoro -h

Will show the help text for each command.
