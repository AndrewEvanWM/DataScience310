For this project, I chose the country of Nepal. I first took in the values from the DHS website and began splitting the data into the correct columns. The hhid, unit, and weights were the same as Professor Frazier's original code. The location was set as $shdist. Then I used the which(colnames(households)... function to determine the correct columns for the sex, age, and education. These three were then pivoted, and more basic formating was done to it. They were then changed to the datatype as.integer so the heatmaps could be printed. Below are the raw, scale, normal, and percent heatmaps for my country of Nepal.

Raw:
![Alt_Text](/raw.png)

Scale:
![Alt_Text](/scale.png)

Normal:
![Alt_Text](/normal.png)

Percent:
![Alt_Text](/percent.png)
