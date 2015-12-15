# Practice 2015 - 09: How Much Longer?

## Background
When the Avengers put Loki in prison, they gave him an incredibly menial task
and told him that if he did it successfully, they would let him out. They
figured this task was so mind-numbingly boring that he would never be able to
do it, so there was little risk.

Specifically, Loki has to count the number of times the hour hand and minute
hand cross each other over a set period of time for a number of different clocks
the Avengers put in the room. However, they all work differently than normal
clocks. Loki wants to write a program that will calculate the answers for him,
so he has more time to plot how to take over Asgard. The format of the clocks
is described below.

Earth’s predominant analog clock design has a circular face, as well as an hour
hand and a minute hand which move smoothly around the clock face. Every
revolution of the minute hand around the clock face indicates that the hour
hand has moved forward one hour. Usually, one revolution around the clock face
represents 12 hours for the hour hand and 60 minutes for the minute hand. For
this problem we are not considering the distinction between AM/PM.

What if clocks had a different number of hours and minutes? Given an analog
clock that represents h hours for the hour hand and m minutes for the minute
hand, as well as a start time and an end time, determine how many times the
minute hand overlaps with the hour hand.

If the minute hand and hour hand overlap at the start time or end time, that
does count as an overlap.

For our clocks, the hour hand and minute hand both move smoothly, even between
minutes. This means that at 0:01, the hour hand is no longer exactly
on the 0 o’clock position.

## Description

### Input
The first line of the file will have an integer, n, which is the number of
test cases in this file.

Each of the next n lines will be a test case containing four integers in the
form h m s e, where h is the number of hours the clock represents, m is the
number of minutes the clock represents, s is the start time in the
form (hours):(minutes), and e is the end time in the form (hours):(minutes).
The integers h and m are guaranteed to be greater than 1. The hours and minutes
that make up s and e can vary in number of digits, depending on the values
of h and m. Hours begin at 0 and end at h − 1.

Each clock will have at most 12 hours and at most 60 minutes.

### Output
For each case, output the number of overlaps there are in the given time range
for the given time system, each on a separate line.

## Sample
### Input
```
2
12 60 0:00 11:59
4 13 2:07 3:05
```

### Output
```
11
1
```
