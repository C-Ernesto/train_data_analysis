# train_data_analysis

This notebook analyzes data recording information about freight train accidents.

Each record in the file contains information about one particular shift that an engineer or conductor worked.  Clock-in and clock-out information, plus many statistics, are provided. The time of clock-in is in the column named 'Start', and this value is given as the number of minutes since midnight.  So if the person clocked-in at 7:00 am, this would be recorded as 420 (60 minutes * 7 o'clock).  The clock-out information is in the column named 'End'.  The column labeled 'FIRMF' is the estimated fatigue level of the person, with values ranging from -10 (really fatigued) to +10 (really alert).

One column, named 'class', is actually the target.  This column contains an integer that can have one of three values:

0: No accident occurred during this shift

1: An accident of type '1' occurred during this shift

2. An accident of type '2' occurred during this shift
