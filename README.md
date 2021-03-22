# electoral_analysis
Utilizing Python to do an electoral analysis 

## Overview of Election Audit
In this analysis we'll be utilizing python to audit data for the electiction commission in order to determine the results of the election.  The analysis consists of 4 main sections: The total count of votes in this election, the audit of votes by candidate and county, the final results of the election, and the announcement of the winner.

## Election-Audit Results: 
  
### - How many votes were cast in this congressional election?
The total count of votes was 369,711. In order to determine the total count of votes on the election, we created a *for* loop to go through all the rows on the *election_ressults.csv* file. 

![image](https://github.com/ejyongc/election_analysis/blob/main/Resources/List%20and%20dictionary%20loop.png)
  
### - Provide a breakdown of the number of votes and the percentage of total votes for each county in the precinct.
In the same *for* loop mentioned above, we were able to extract the *candidate_name* & *county_name* into two separate lists, and *candidates_votes* and *counties_votes* into two separate dictionaries that will be used later to calculate the votes and percentage of total votes for each county and candidate.
  
After creating the list and dictionary for the counties, we ran a loop to calculate *votes* and *votes_percentage* for each county in the *county_name* list. (image below)

![image](https://github.com/ejyongc/election_analysis/blob/main/Resources/Loop%20for%20counties.png)
  
After printing the results on the terminal and the *election_analysis.txt* file, we can see that the *Denver* county got the majority of the votes by a big difference (306,055 or 82.8% of the total votes). *Jefferson* county got 38,855 votes (10.5%) while Arapahoe casted 24,801 (6.7%) votes. 
  
### - Which county had the largest number of votes?
As mentioned earlier, *Denver* is the county with the largest turnout in terms on votes. We utilized an *if* statement to calculate the *county_winnnig_count, winning_county, and county_winning_percentage*
  
### - Provide a breakdown of the number of votes and the percentage of the total votes each candidate received.
Very similarly to the *for* loop we created to calculate the results for each county, we created a *for* loop to calculate the count of votes and percentage of votes for each candidate.
The results indicate that *Charles Casper Stockham* received 85,213 votes which represent 23.0% of the total votes.  *Diana DeGette* received 272,892 votes (73.8%), and finally *Raymond Anthony Doane* received the least amount of votes at 11,606 (3.1%). 
  
![image](https://github.com/ejyongc/election_analysis/blob/main/Resources/loop%20for%20candidates.png)
  
### - Which candidate won the election, what was their vote count, and what was their percentage of the total votes?
As we can see from the results above, *Diane DeGette* is the candidate that won the election by a great advantage against her adversaries. Her final vote count was 272,892 which represented 73.8% of all the votes. 
  
We calculated the *winning_count, winning_candidate, and winning_percentage* by running an *if* statement at the end of the *for* loop. 
  
## Election-Audit Summary: 
In a summary statement, provide a business proposal to the election commission on how this script can be used—with some modifications—for any election. Give at least two examples of how this script can be modified to be used for other elections.

Finally, the results of this election shown above is based on the dataset provided on the file *election_results.csv* but they are not limited to this dataset. This script can be utilized to audit different election results as the *file_to_load* variable could be modified to load a file from a different path (line 09 - Image below)

![image](https://github.com/ejyongc/election_analysis/blob/main/Resources/file%20to%20open.png)

