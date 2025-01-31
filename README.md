# Birthday Problem

The purpose of this challenge is to continue practicing with input and output, converting to integers,
and in particular with writing programs that use *conditionals* to make decisions.

Your program will ask the user the following questions, in this order:

1. Their name.
2. The name of the month they were born in (e.g. "September").
3. The year they were born in (e.g. "1962").
4. The day they were born on (e.g. "11").

If the user's birthday fell on October 31, then respond with:

```You were born on Halloween!```

If the user's birthday fell on today's date, then respond with:

```Happy birthday!```

Otherwise respond with a statement like this:

''```Peter, you are a winter baby of the nineties.```''

## Example Session

So a typical session would look like this (remember: details matter!)

    Hello, what is your name? Eric
    Hi Eric, what was the name of the month you were born in? September
    And what year were you born in, Eric? 1972
    And the day? 11
    Eric, you are a fall baby of the Stone Age.

## Some Definitions

Winter (```winter```) babies were born in months of December through February.

Spring (```spring```) babies were born in months of March through May.

Summer (```summer```) babies were born in the months of June through August.

Fall (```fall```) babies were born in the months of September through November.

Years from 1980-1989 are known as the ```eighties```.

Years from 1990-1999 are known as the ```nineties```.

Years from 2000 through today are known as the ```two thousands```.

Years prior to 1980 are known as the ```Stone Age```.

## Useful Tips

You will find it useful to import a couple of libraries related to dates: import the ```datetime```
function from ```datetime``` and the ```month_name``` name from ```calendar```.

Then you can get today's month (as a number) and date using:

```python
from datetime import datetime
from calendar import month_name
todaymonth = datetime.today().month
todaydate = datetime.today().day
```

And you can get the name of a month from its number using something like:

```python
month = month_name[todaymonth]
```
