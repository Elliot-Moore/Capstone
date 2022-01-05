Executive Summary

I enjoy chess, so I focused my Capstone project on analyzing chess openings using Python. My goal is to use current chess opening data to recommend openings that are uncommon and leave common chess opening theory quickly. I will be using a chess database of master level games for this analysis. 
Motivation

I have been a huge chess nerd for many years- I follow the latest chess news, enjoy playing chess and some of its variants, and am especially fascinated with computer chess- that is, chess engines playing each other and the games they produce. I’m the kind of person who likes to see hard data with everything, and chess is no exception. One area with extensive numbers and records in chess is the opening phase of the game, which fit perfectly as the subject of my Capstone project. 
Data Question

Can I use data analysis on chess openings to find the best openings for a human player to use to avoid chess opening theory? 
Chess opening knowledge has expanded over the years as players get stronger and 
new resources emerge, such as online databases and chess engines. As theory has expanded it becomes more and more difficult for players at the top level to gain an advantage out of the opening- a strong chess grandmaster will simply know so much theory it can seem impossible to ever surprise them- much less beat them. Many players, such as World Chess Champion Magnus Carlsen, do their best avoid the expected and play the unexpected, because the expected has been analyzed too deeply (link). As the great chess player Mikhail Tal put it, “You must take your opponent into a deep dark forest where 2+2=5, and the path leading out is only wide enough for one”. Most of the time, strong players use personal intuition and research to find these tricky moves- not necessarily the best move, but the move most likely to beat the opponent. This leads to my question- can this be done using data analysis with a program instead? This approach has probably been tried, but I’m not knowledgeable of any such attempts. 

Minimum Viable Product (MVP)

The finished product will be a database with popular chess openings scored based primarily on the ability to diverge from standard opening theory as quickly as possible without sacrificing too much in opening solidity. Visualizations demonstrating the scoring system’s ability to find these moves will be provided via PowerPoint or similar visual medium. The intended audience are serious chess players looking for new opening ideas.

Schedule (through 1/7/2022)

1.	Get the Data (12/10/2021)
2.	Clean & Explore the Data (12/14/2021)
3.	Create Presentation of your Analysis (1/5/2022)
-	Should be a presentation, but could include a Jupyter Notebook or dashboard in Excel, Tableau, or PowerBI
4.	Internal demos (12/17/2021)
5.	Demo Day!! (1/7/2022)

Data Sources

Caissabase- a free regularly updated chess database containing around 4.56 million chess master level games. This database combines several other databases and sources of games to be as all-encompassing as possible, which was very helpful for me. I solely used Caissabase for my game data. 
Known Issues and Challenges

Chess game data is readily available via many free online databases, so getting the data is not an issue. 

Some issues I ran into:
•	The dataset was large enough to be problematic in an of itself- my code frequently ran slowly, and I had to be careful the order in which I ran my code to avoid running out of space on my computer.
•	After getting the data into a format useable in Python, the data for each game was in string format with no separations, so I had to make careful use of Python regex to pull out each piece of information. It was especially tricky to separate out opening moves from standard chess notation into separate columns in a Pandas dataframe. 
