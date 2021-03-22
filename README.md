# electoral_analysis
Utilizing Python to do an electoral analysis 




1. Overview of Election Audit: Explain the purpose of this election audit analysis.

### Analysis Overview and Purpose
In this analysis we'll be utilizing python to audit election data for the electiction commission in order to determine the results of the election.  The analysis consists of 3 main sections: The total count of votes in this election, the audit of votes by candidate and county, and the final results of the election and the announcement of the winner.

2. Election-Audit Results: 
Using a bulleted list, address the following election outcomes. Use images or examples of your code as support where necessary.
  
  #### - How many votes were cast in this congressional election?
  The total count of votes was 369,711. In order to determine the total count of votes on the election, we created a loop to go through all the rows on the *election_ressults.csv* file. 
  
  #### - Provide a breakdown of the number of votes and the percentage of total votes for each county in the precinct.
  In the same loop we extracted the *candidate_name* & *county_name* into two separate list, and *candidates_votes* and *counties_votes* into two separate dictionaries that'd be later used to calculate votes and percentage of total votes for each county and candates.
  
  
  #### - Which county had the largest number of votes?
  #### - Provide a breakdown of the number of votes and the percentage of the total votes each candidate received.
  #### - Which candidate won the election, what was their vote count, and what was their percentage of the total votes?

3. Election-Audit Summary: In a summary statement, provide a business proposal to the election commission on how this script can be used—with some modifications—for any election. Give at least two examples of how this script can be modified to be used for other elections. 

