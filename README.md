# API Data Analysis Using Python Structures

The goal of this project was to fetch a customer directory from an API, explore its nested structure and answer simple distribution questions with sets, dicts and a chart.

### Explore nested dictionaries and lists
Indented Attributes:
- address
- geo
- company
  
The deepest attributes are lat and lng which are nested inside geo, which is inside the address.
The `explore` function begins at indentation level zero and recursively explores all nested dictionaries until the deepest one.


### Visualise the customer distribution
For now, no chart is more useful than the other because every single instance in the dataset occurs exactly once, i.e uniform distribution.