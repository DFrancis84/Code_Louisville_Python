# <p align="center"> Code Louisville 2018 Python Project - Devin Francis </p>


## To Install
```
git clone https://github.com/DFrancis84/Code_Louisville_Python.git
```

## You will need the following dependencies/programs
1. Anaconda - https://www.anaconda.com/download
2. Jupyter Notebook - http://jupyter.org/install
3. SQLite3 - https://www.tutorialspoint.com/sqlite/sqlite_installation.htm
4. Pandas - https://pandas.pydata.org/
5. Numpy - https://scipy.org/install.html
6. Matplotlib.pyplot - https://matplotlib.org/users/installing.html
7. RISE - https://github.com/damianavila/RISE

## To Run
1. Open your terminal
2. Run Jupyter Notebook via `jupyter notebook`
3. Select `Code Louisville 2018 Project` from your selections
4. Open `Code_Louisville_Project.ipynb` file
5. Click **RUN** (this will cause all the code to be hidden and just display the slides)
    * If you want to view the code; Just click the **Show Code** button at top of notebook
6. Click the statistics bar located at the very end.  This will only be present once you have RISE installed.  It will begin the slideshow presentation.
7. Use **RIGHT** arrow to move slides forwards, and use **LEFT** arrow to move slides backwards.  There are no subslides, so the use of the **DOWN** arrow will not be needed.

## DATA DICTIONARY
```
    RANK - MLB RANK IN 2017
    TEAM - TEAMS IN THE MLB
    AB - AT BATS
    R - RUNS
    H - HITS
    HBP - HIT BY PITCH
    E - ERRORS
    AVG - AVERAGE
    SLG - SLUGGING PERCENTAGE
    OBP - ON BASE PERCENTAGE
    RUNRATIO - CALCULATED FORMULA, HITS DIVIDED BY RUNS
    LHP - LEFT HANDED PITCHER
    RHP - RIGHT HANDED PITCHER
```



## Which is the tougher matchup? Left-Handed Pitchers(LHP) or Right-Handed Pitchers(RHP)?


For my project, I used `MLB.com` to download the data from the 2017 season to help answer the age old question of, "Is a LHP better than a RHP?".

In the MLB there are less left-handed batters than right-handed in the lineups so that means that left-handed pitchers have more advantage then righties.  So that is why you hear the phrase, "A lefty is better than a righty".  I wanted to put that to the test and use the numbers to see if the statement is in fact "True".

In order to put this to the test, I used three different sets of data.
1. Batting Averages
2. Runs per Hit (Run Ratio)
3. Actual average amount of runs given up per AB

First; I used the actual batting averages against each individual pitcher. I took the data from all 30 teams, and combined them together.  Using SQLite, I took that data and got the average batting average amongst all teams, per pitcher.  I then graphed all 30 teams against the league average. The results were inconclusive as it was dispersed against both pitchers.

Second; I used the average runs scored per hit against each pitcher. To get this data I gathered all the runs and hits for the entire league.  By dividing the two together, I was able to come up with a league average.  I graphed the individual teams average runs per hit against the determined league average.  Same as the data before, the results did not heavily favor one or the other.  

Finally; I went for all the glory and decided to see which pitcher gave up the most runs per AB.  At Bat is defined as "a player's turn at batting, as officially recorded".  Which means that anytime a batter steps into the batter's box, they are considered At Bat.  This statistic takes into effect outs, walks, hbp, e, along with hits. Even though the results were close, clearly if one pitcher gave up more runs than the other, then that would determine if one was better than the other. 

Go ahead and give the file a run to see the results.... What do you think the answer will be?  Is a LHP better than a RHP?
