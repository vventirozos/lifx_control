# Lifx tools
Simple command line tool for controlling Lifx light bulbs based on lifxlan. Supports turning it
on and off, colors and preset profiles for day, evening and night with whites
with different brightness and temperature. It also supports an "auto" mode
which will determine location and sunset (ip based) and it will apply a preset schedule.
The current (hardcoded) schedule is:
From 9:30am to sunset-2hours day mode,
Fron sunset-2hours to sunset+2hours	evening mode,
From suset+2hours to 9:30am	night mode.
These are easy to change, see function autodim in the script.
It should be working for more than one lamp, but i haven't tested it. I assume it will apply the same
changes to all, one by one.
It won't apply any changes to any lamps that are not 'on' but it shouldn't error if
lamp is off from the switch. which makes "auto" ideal for crontab.
