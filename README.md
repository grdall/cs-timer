# C# Timer

A C# program with possibility to set multiple asynchronous timers.

## Usage (Windows)
1. [Install Mono](https://www.mono-project.com/download/stable/) to compile the code
2. Make sure Mono is defined on PATH
3. Navigate to folder in CLI
4. $ `mcs timer.cs`
5. $ `./timer.exe [flag flagvalues, ...]`

Alternativly, download the .exe and run from commandline like point 5.

Note: ? indicates optional arguments.

### Arguments:

| Arument | Flags | Details |
| --- | --- | --- |
| -timer, -t | ?[time-unit] + [time] + ?"[message]" | sets a timer for [time] with [time-unit] value in minutes with the message [message] |
| -stopwatch, -sw | none | starts a stopwatch (Spacebar to pause) |
| -convert, -c | [time-unit] + [time] + [to-time-unit] | converts time from [time-unit] to [to-time-unit] |
| -help, -h | none | prints this usage guide |

### Examples

| Goal | Command |
| --- | --- |
| Set a timer for 10 seconds:                      | $ `./timer.exe -t s 10 "Count to 10 finished"` |
| Set a timer for 8.5 minutes:                     | $ `./timer.exe -t m 8.5 "Eggs are done"` |
| Set a timer for 1 hour:                          | $ `./timer.exe -t h 1 "Remember to stand up every hour"` |
| Set a timer for 5 minutes:                       | $ `./timer.exe -t 5 alarm` |
| Set a timer for 2 hours, 30 minutes, 15 seconds: | $ `./timer.exe -t h 2 m 30 s 15` |

## My Thoughts

Having the usefulness of a timer I could use while working on my computer was something that was validated after I made a C++ timer, however, 
it was janky and hand issues, not including the headache of getting C++ to work properly. After not being able to compile by the compiler, 
I thought I might as well try C#, which is another language I want more experience with. I took the good aspects of the previous project and 
implemented and improved them in this project.

## TODO

- Flashing icon or bringing visual attention to window (important)
- Settings file? Options to have alarm sound on loop
- timer + time/message in window title box
- make program ignore when clicking somewhere in window, disrupting timer
- spellcheck