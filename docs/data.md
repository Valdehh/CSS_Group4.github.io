---
layout: default
---

# Data
To collect the data API calls was made to the base URL https://api.github.com. Firstly, search calls were made to repositories who contained topics of Machine learning and Deep learning. This provided us with 1509 of the most popular repositories within these two categories sorted by GitHub stars. 

Then using the same Base URL we called for the repositories to get the owners and all contributors. Based on the API calls a dataframe is created containing:

- Repository name
- Repository owner and name
- List of contributors
- Repository topics
- Repository descriptons
- Repository ReadMe files
- Repository Stargazer count
- Status code

Furthermore, a data frame is created linking each contributor to a company. The data used in this project is ready made data, it is expressed as the data is collected from open-source repositories resulting in a large portion of the accounts are private. This results in the company attribute is missing for a large part of the data and that companies often are spelled differently. If a contributor has not indicated a company a unique index was given to set contributor. As many companies was spelled different and the large number of empty company fields we ended up with 17349 unique companies in the network.