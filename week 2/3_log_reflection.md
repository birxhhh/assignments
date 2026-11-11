Assignment 2: Reflection Log

               (CODE)                                 (AI ACTION)                            (VERDICT)          (EVIDENCE)                
 (1)Price Data Type Conversion(`pd.to_numeric`) ==  Converts string prices to numeric floats == Keep    == It successfully converted objects to float which I confirmed via .describe().
 (2)Duplicate Row Removal(drop_duplicates())    ==  Drops identical duplicate row            == Keep    == It removed the duplicates properyand I verified row counts before and after using .shape()
 (3)Missing Price Hanlding                      ==  It blindly suggested to delete it        == Reject  == Instead of blindly dropping rows with missing prices, I flagged them for future users.

2. Comparison of Decisions: 
Where our decisions differed: 

-The AI suggested dropping rows with missing values or weird string characters automatically. I decided to flag rather than blindly delete.
Which was better supported:
My decision was better supported because it maintained data transparency.

3. What Would Have Been Missed Alone?

Working through this audit alone helped me catch formatting issues and I had to consistently check using .describe()
However using the AI as a coach helped in identifying the syntax that saved time on syntax troubleshooting, which allowed me to focus entirely on assessing whether the code was safe to run instead of me having to write it form scratch.