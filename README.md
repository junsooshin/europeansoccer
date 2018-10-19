# European Soccer Goal Data Exploration

By **Derek Shin**

October 2018

* * *

#### Motivation

The main European soccer dataset is from [https://www.kaggle.com/hugomathien/soccer/home], and the supplementary dataset that includes the goal type is from [https://www.kaggle.com/jiezi2004/soccer/home].

The dataset covers the seasons from 2008 to 2016 (from the 2008/09 season to the 2015/16 season).<br>
The goals are just for the domestic league matches.

Question 1: Who scores most of their goals through penalty kicks?<br>
Question 2: When are the goals scored?

* * *

#### Motivation
Soccer is a sport that doesn't allow many points, or goals. That's why the fans clap for a hard tackle, which turns out to be a foul, and cheer for a long pass across the field that may or may not push the play forward. That's why the players get high-fives from their teammates after hitting a goal post with their shots and the goalkeepers yell at their defenders even after looking at a shot go way above his head -- it just shouldn't even be close.

And there is penalty kick. It's the easiest, most certain way to score a goal. You place the ball 12 yards away from the goal line and smash it past the goalkeeper standing in front of a rectangular goal that is 24 feet wide and 8 feet high. Scoring a penalty kick ([83.4%](http://www.myfootballfacts.com/Premier_League_Penalty_Statistics.html) for the Premier League from 92/93 to 17/18) is a bit easier than making a free throw ([76.7%](https://www.basketball-reference.com/leagues/NBA_stats.html) in the 2017/18 NBA regular season) and a little harder than converting the extra-point kick after a touchdown ([94%](http://www.espn.com/nfl/statistics/team/_/stat/kicking/sort/extraPointPct/position/defense/year/2017) in the 2017 NFL regular season). But a penalty kick is not 1 point out of a hundred in a basketball game or 1/7 of an actual goal (touchdown) in American football——it often changes the outcome of a soccer match. So, if you are taking a penalty kick, you have to score.

I've noticed some unlikely penalty kick takers, such as James Milner for Liverpool and, before, Leighton Baines for Everton. They must have practiced a lot after their training sessions and proven their skills, but I was surprised nontheless because they are not prolific strikers or attacking midfielders who score 10+ goals every season and possess amazing kicking abilities like Steven Gerrard or Frank Lampard.

So, I wanted to see who scored most of their goals through penalty kicks––the players who would have much lower goal tallies if they weren't the designated penalty kick takers for their clubs but honed their crafts and left their marks.

* * *

#### Conclusion

**Things I learned from answering question 1**
- Penalty kick goals are rare: 7.9% of all goals.
- Some teams don't even score one for the entire season, while some score 13. The average is 3.8 penalty kicks per team, per season.
- Defenders and non-offensive midfielders score most of their goals via penalty kicks: Fabinho, Siqueira, Verhaegh, Murphy.
- Filip Daems (1 normal goal, 12 pk) and Paul Verhaegh (2 normal goals, 14 pk) were the best ones in this category.
- The target strikers who might not be the best penalty kick takers, such as Mario Gomez (100 normal goals, 6 pk), Stefan Kiessling (102 normal goals, 7 pk), and Fernando Llorente (86 normal goals, 6 pk) were at the bottom of the list.

**Things I learned from answering question 2**
- More goals are scored as the matches go on: the goal totals and the time they were scored have a ~0.85 correlation.
- Much less goals (about half less than any other minutes) are scored on the 1st and 46th minutes of the matches.
- Relative proportion of penalty kick goals are higher than that of normal goals in the second half. (24:20)

* * *

#### Sources that helped me

**Stack Overflow**
- [Select rows from a DataFrame based on values in a column in pandas](https://stackoverflow.com/questions/17071871/select-rows-from-a-dataframe-based-on-values-in-a-column-in-pandas)
- [How to change the order of DataFrame columns?](https://stackoverflow.com/questions/13148429/how-to-change-the-order-of-dataframe-columns)
- [How to merge two dataframes side-by-side?](https://stackoverflow.com/questions/23891575/how-to-merge-two-dataframes-side-by-side)
- [Select rows from a DataFrame based on values in a column in pandas](https://stackoverflow.com/questions/17071871/select-rows-from-a-dataframe-based-on-values-in-a-column-in-pandas)
- [Plotting value_counts() in seaborn barplot](https://stackoverflow.com/questions/31460146/plotting-value-counts-in-seaborn-barplot)
- [How do you change the size of figures drawn with matplotlib?](https://stackoverflow.com/questions/332289/how-do-you-change-the-size-of-figures-drawn-with-matplotlib)
- [Sort by index in value_counts()](https://stackoverflow.com/questions/43855474/changing-sort-in-value-counts)
- [Seaborn Barplot - Displaying Values](https://stackoverflow.com/questions/43214978/seaborn-barplot-displaying-values)
- [Add zeros to a float after the decimal point in Python](https://stackoverflow.com/questions/15619096/add-zeros-to-a-float-after-the-decimal-point-in-python)
- [Replace all the NaN values with Zero's in a column of a pandas dataframe](https://stackoverflow.com/questions/13295735/how-can-i-replace-all-the-nan-values-with-zeros-in-a-column-of-a-pandas-datafra)
- [Pandas: change data type of Series to String](https://stackoverflow.com/questions/22231592/pandas-change-data-type-of-series-to-string)
- [How to save a Seaborn plot into a file](https://stackoverflow.com/questions/32244753/how-to-save-a-seaborn-plot-into-a-file)
- [Get the max of each group when using groupby()](https://stackoverflow.com/questions/44555579/get-the-max-of-each-group-when-using-groupby-on-two-columns-python)
- [How do I set the figure title and axes labels font size in Matplotlib?](https://stackoverflow.com/questions/12444716/how-do-i-set-the-figure-title-and-axes-labels-font-size-in-matplotlib)
- [Compare two columns using pandas](https://stackoverflow.com/questions/27474921/compare-two-columns-using-pandas)

**Pandas**
- [pandas.Series.str.contains](https://pandas.pydata.org/pandas-docs/stable/generated/pandas.Series.str.contains.html)
- [pandas.Series.str.slice](https://pandas.pydata.org/pandas-docs/stable/generated/pandas.Series.str.slice.html)
- [pandas.Series.value_counts (`normalize` parameter)](https://pandas.pydata.org/pandas-docs/stable/generated/pandas.Series.value_counts.html)
- [renaming a column](http://pandas.pydata.org/pandas-docs/stable/basics.html#basics-rename)
- [pandas.DataFrame.reset_index](https://pandas.pydata.org/pandas-docs/stable/generated/pandas.DataFrame.reset_index.html#pandas.DataFrame.reset_index)
- [pandas.DataFrame.sort_values](https://pandas.pydata.org/pandas-docs/stable/generated/pandas.DataFrame.sort_values.html)