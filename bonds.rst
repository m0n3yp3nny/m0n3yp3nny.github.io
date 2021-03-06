.. _bonds:

******
Investigating Revolutionary War bonds
******

During the American Revolution, bonds were issued by the Patriot forces to fund campaigns. The records for these loans existed in handwritten ledgers from the 1770s and 80s, and was keyed into Excel. We took these Excel sheets and created data frames, using plotly to find patterns in the data.

The loans were later restructured under Alexander Hamilton, which you can read about in the `First Report on the Public Credit`_.

.. _First Report on the Public Credit: https://en.wikipedia.org/wiki/First_Report_on_the_Public_Credit

We have created a number of graphs to initially investigate the data. In order to see how these loans changed hands over time, however, we need a method for matching same and similar names across data frames.

In order to do this, we plan to use the `fuzzywuzzy`_ package for Python. Because of the nature of the original ledgers, differences in spelling is common, as well as loans being passed between family members or sold. This will present a challenge for the fuzzy matching algorithm.

.. _fuzzywuzzy: https://github.com/seatgeek/fuzzywuzzy

The bonds were initially extended by separate colonies, so our data is structured to separate loans by principle amount and by colony. Rhode Island has the smallest number, so we started there.
