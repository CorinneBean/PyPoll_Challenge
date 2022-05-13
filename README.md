# PyPoll_Challenge

## Overview of Election Audit
The purpose of this audit is to review local congressional election results for the Colorado Board of Elections. The election commission requested additional data to complete the audit.

The following additional data was requested for this audit:
- The voter turnout for each county
- The percentage of votes from each county out of the total count
- the county with the highest turnout

## Election Audit Results
After careful analysis the followng information was found during the audit.

### Voter Turnout by County
```
Jefferson: 38,855
Denver: 306,055
Arapahoe: 24,801
```
### Percentage of votes by County
```
Jefferson: 10.5%
Denver: 82.8%
Arapahoe: 6.7%
```
### Largest County Turnout
```
Denver: 306,055
```

## Election Audit Summary

The following code reviews the election_results.csv file to determine each counties voter turnout. As long as the .csv file used for the analysis contains the following structure it should function as intended for any election.
```
Ballot ID | County | Candidate
```

- Modifying Code
> Currently the code is set to create a ist of county names and a dictionary of county votes from the .csv file. 
```py

county_names_list = []
county_votes_dict = {}
``` 
> This flexibily makes this code versitile to be used in any election as long as the .csv file is structured in the manner mentioned above. However, if one would wish to review only voting data for specific counties they can edit the code as follows:

```py

county_names_list = ["enter county name here"]

``
