# Election_Analysis

## Project Overview
A Colorado Board of Elections employee has given us the following tasks to complete the election audit of a recent local congressional election.

1. Calculate the total number of votes cast.
2. Get a complete list of candidates who received votes.
3. Calculate the total number of votes each candidate received.
4. Calculate the percentage of votes each candidate won.
5. Determine the winner of the election based on popular vote.

This analysis is intended to tally individual ballots recorded in a CSV file containing a ballot ID, county, and candidate. The analysis counts the total number of votes cast, votes by candidate, and voter turnout by county. By counting candidate votes we also determine the winner of the vote.

## Resources
- Data Source: `election_results.csv`
- Software: Python 3.7.6, Visual Studio Code 1.63.1

## Election Audit Results
The analysis of the election shows that:

* There were 369,711 votes cast in the election.
* Voter turnout by county was as follows:
  * Jefferson: 10.5% (38,855 votes)
  * Denver: 82.8% (306,055 votes)
  * Arapahoe: 6.7% (24,801 votes)
* Denver county had the largest number of votes at 306,055.
* Candidate vote results were as follows:
  * Charles Casper Stockham: 23.0% (85,213 votes)
  * Diana DeGette: 73.8% (272,892 votes)
  * Raymon Anthony Doane: 3.1% (11,606 votes)
* The winner of the election was Diana DeGette, who received 272,892 votes representing 73.8% of the overall votes.

These results are printed to the terminal and saved to a file, `election_analysis.txt`.

## Election Audit Summary

The audit code works for the specific format provided for this congressional election. To generalize the solution so it can be applied to other elections, such as senatorial or mayoral elections, some changes might be required. For example, the source might not include a county name, or might record whether a vote was hand-counted or machine-counted. Therefore, the code should be improved by validating the headers provided with the CSV source file to ensure columns are included in the expected order (or selecting different indexes based on the actual column headers).

Another improvement to consider might be to include candidate party affiliation in the results. This could be achieved by adding a second source file with a list of candidates and their parties, or by adding an extra column to the `election_results.csv` file. The party name could then be incorporated into the output.
