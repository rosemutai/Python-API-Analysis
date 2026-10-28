# API Data Analysis Using Python Structures

The goal of this project was to fetch a customer directory from an API, explore its nested structure and answer simple distribution questions with sets, dicts and a chart.

## Python skills
- Requests & APIs
- JSON
- Dictionaries
- Sets
- Comprehensions
- Pandas
- Data visualization

### Prerequisites

An understanding of Python 

### Install

In order to run this project you need to have the following:
- A code editor (VSCode)

### Setup

To get a local copy up and running follow these simple example steps:
- Open git bash on a local computer
- clone the repo with: 
  
```
git clone  <https://github.com/rosemutai/Python-API-Analysis>
```

- run ```cd Python-API-Analysis-main``` to enter the project folder
- run ```pip install -r requirements.txt``` to install all dependencies
- Click `Run All` to run the `analysis.ipynb` file

## Analysis

### Explore nested dictionaries and lists

Indented Attributes:
- address
- geo
- company
  
The deepest attributes are lat and lng which are nested inside geo, which is inside the address.
The `explore` function begins at indentation level zero and recursively explores all nested dictionaries until the deepest one.

### Extract customer attributes

Implemented extract_attributes(customers) to extract id, name, username, email, email_domain, phone, city, zipcode, latitude, longitude, company and website then transformed nested records into a flat dictionary for each customer.

### Use sets to find unique cities

There are 10 unique cities and 10 customers.
For marketing, this shows that the customers are dispersed geographically hence the need to account for different locations instead of just focusing on one location.

### Visualise the customer distribution

The email domain chart is more useful because repeated domains can reveal common email providers among customers compared to cities.

## Assumptions

1. Each record represents a distinct customer.
2. A customer's city is their main location no matter where they work.
3. Email domains are extracted correctly, the domain is assumed to be after '@' symbol.