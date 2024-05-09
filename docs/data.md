---
layout: default
---

# Data
To collect the data API calls was made to the base URL https://api.github.com. Firstly, search calls were made to repositories who contained topics of Machine learning and Deep learning. This provided us with 1510 of the most popular repositories within these two categories sorted by GitHub stars. 

Then using the same Base URL we called for the repositories to get the owners and all contributors. Based on the API calls a dataframe is created containing:

<ul style="list-style-type:circle; font-family: Arial, sans-serif; font-size: 1.2em; color: #333;">
  <li>Repository name</li>
  <li>Repository owner and name</li>
  <li>List of contributors</li>
  <li>Repository topics</li>
  <li>Repository descriptions</li>
  <li>Repository ReadMe files</li>
  <li>Repository Stargazer count</li>
  <li>Status code</li>
</ul>

Number of unique companies: 40443