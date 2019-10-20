# cs-timer

A C# program with possibility to set multiple asynchronous timers.

## Usage (Windows)
1. [Install Mono](https://www.mono-project.com/download/stable/) to compile the code
2. Make sure Mono is defined on PATH
3. Navigate to folder in CLI
4. $ mcs timer.cs
5. ./timer.exe [flag flagvalues, ...]

Alternativly, download the .exe and run from commandline like point 5.

Flags:
- -time, -t + [time] + "[message]": sets a timer for [time] value in minutes with the message [message]
    - Examples: 
        - Set a timer for 8.5 minutes: $ ./timer.exe -t 8.5 "Eggs are done"
        - Set a timer for 1 hour: $ ./timer.exe -t 60 "Remember to stand up every hour"
- -stopwatch, -sw: starts a stopwatch
- -help, -h: prints this usage guide


## TODO

- Flashing icon or bringing visual attention to window
- Resize window to fit better for small text usage
- option to use seconds/minutes/hours
- stopwatch
- timer + time/message in window title box
- make program ignore when clicking somewhere in window, disrupting timer
- clean up "using.."
- spellcheck

## My Thoughts

Having the usefulness of a timer I could use while working on my computer was something that was validated after I made a C++ timer, however, it was janky and hand issues, not including the headache of getting C++ to work properly. After not being able to compile by the compiler, I thought I might as well try C#, which is another language I want more experience with. I took the good aspects of the previous project and implemented and improved them in this project.