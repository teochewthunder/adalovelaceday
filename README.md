# Ada Lovelace Day Generator
This code is a component that generates Ada Lovelace Day (second Tuesday of October) for the given year. The default is the current year.

*year* and *adaLovelaceDay* are stored in state. The idea is when these change, the display changes.

*digitGen* is a cmponent that comprises of **four** sub-components which in turn comprise of a number and two buttons - one to increment the number and one to decrement. Clicking on these buttons will change their assigned number, and this in turn will trigger a change in the *year*, which will then trigger the *showAdaLovelaceDayForYear()* method.

## *showAdaLovelaceDayForYear()* method
This method accepts a year and generates the date of the second Tuesday of October in that year. The code for this is not 100% optimized, though maybe it doesn't need to be. It basically starts from the first day of October and increments till it reaches the second Tuesday.

*Note:* For loops don't work in the *render()* method, thus I had to use an array with the *map()* method.
