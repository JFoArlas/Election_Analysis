# Election_Analysis

## Project Overview
The Colorado Board of Elections requested a summary of the following election results:

1. Total number of votes cast
2. List of candidates who received votes
3. Total number of votes per candidate
4. Percentage of votes per candidate
5. Winner of the election based on the popular vote

## Resources
- Data Source: election_results.csv
- Software: Python 3.8.9, Visual Studio Code, 1.60.2

## Summary
- Total votes cast: 369,711
- Outcome (# and % of votes per candidate):
  - Charles Casper Stockham: 23.0% (85,213 votes)
  - Diana DeGette: 73.8% (272,892 votes)
  - Raymon Anthony Doane: 3.1% (11,606 votes)
- Winner: Diana DeGette with 73.8% (272,892 votes)

# Challenge Overview

## Overview of Election Audit
The challenge was to write python code to read a .csv file of election results, and write a summary of the results to a text file. The .csv file of election results included a Ballot ID, county of the voter, and the name of the candidate they voted for. The results summary needed to contain the total number of votes, as well as the vote count for each county and candidate. It also needed to include the percentage of votes for each county and candidate. Lastly, it needed to identify which county had the highest voter turnout and which candidate won based on the popular vote.

## Election-Audit Results
- There were 369,711 votes cast in this congressional election
- County Results (# and % of votes per county):
  - Jefferson: 10.5% (38,855)
  - Denver: 82.8% (306,055)
  - Arapahoe: 6.7% (24,801) 
- Denver county had the largest number of votes
- Candidate Results (# and % of votes per candidate):
  - Charles Casper Stockham: 23.0% (85,213 votes)
  - Diana DeGette: 73.8% (272,892 votes)
  - Raymon Anthony Doane: 3.1% (11,606 votes)
- Diana DeGette was the winner with 73.8% of the total votes cast (272,892 votes)

# Challenge Summary

## Election-Audit Summary

This script can be applied to calculate and summarize the results of any election and can be customized accordingly. For example, if you're looking to calculate results of a different type of election (e.g., state vs. county), you can simply replace "County" with "State" in the script. This would result in the script functioning in the same way, but the text file (and terminal) would appropriately indicate the results were for a state election.

Additionally, this script can be modified to identify the candidate and county with the most votes by using `max_candidate = max(candidate_votes, key=candidate_votes.get)` and `max_county = max(county_votes, key=county_votes.get)` [(ref).](https://www.kite.com/python/answers/how-to-find-the-max-value-in-a-dictionary-in-python) This would identify the county or candidate key with the max value in the respective dictionary.
