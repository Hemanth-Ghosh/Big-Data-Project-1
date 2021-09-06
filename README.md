# Wikipedia Big Data Analysis
###### By: Hemanth Ghosh

## Project Description

This analysis consists of using big data tools to answer questions about datasets from Wikipedia. There are a series of analysis questions, answered using Hive and MapReduce. The tools used are determined based on the context for each question.

## Technologies Used

1.  Hadoop
2.  HDFS
3.  Python
4.  Hive
5.  MapReduce
6.  Yarn
7.  Git + Github

## Features (Problem Statements)

1. Which English wikipedia article got the most traffic on January 20, 2021? 
2. What English wikipedia article has the highest views of its readers follow an internal link to another wikipedia article?
3. What series of wikipedia articles, starting with Hotel California, keeps the highest views of its readers clicking on internal links.
4. Find an example of an English wikipedia article that is relatively more popular in the Americas than elsewhere.There is no location data associated with the wikipedia pageviews    data, but there are timestamps. 
5. Find which device(PC or Mobile) generates the most traffic on the English Wikipedia article?



## Getting Started

Most of the code was done using HQL in a Hive GUI interface via Data Analysis studio or CIL of root@sandbox.

* Download Hortonworks community Edition -https://www.cloudera.com/downloads/hortonworks-sandbox/hdp.html
* Install Hortonworks on your machine or virtual machine - https://www.virtualbox.org/wiki/Downloads
* Download Git Bash on your computer - https://git-scm.com/downloads
* Clone my code - git clone https://github.com/Hemanth-Ghosh/Big-Data-Project-1.git
* Setup the Hortonworks in virtual machine, import pageviews and clickstream data in hdfs, and start query in the CIL or DAS of hive.


## Data Definitions

    For Problem Statement 1, 4 & 5 we need to Download jan 20, 2021 DataSet.
    eg: fr.b 1-Naphthol 1 737**

### Data Explanation

domain_code: fr.b

page_title: Naphthol

count_views: 1

total_response_size: 733

### Types Of Data

wikibooks: ".b"         
wiktionary: ".d" 
foundationwiki: ".f"         
mobile sites: ".m" 
wikinews: ".n"          
wikiquote: ".q"
wikisource: ".s"         
wikiversity: ".v" 
wikivoyage: ".voy"       
mediawikiwiki: ".w" 
wikidatawiki: ".wd" 

    For Problem Statement 2 & 3 we need to download Jan 2021 month DataSet.
    eg: other-search Camp_Tawonga external 183

### Data Explanation

prev: the result of mapping the referrer URL to the fixed set of values described above

curr: the title of the article the client requested

type: describes (prev, curr)

n: the number of occurrences of the (referrer, resource) pair

### Types Of Data

type: describes (prev, curr)

link: if the referrer and request are both articles and the referrer links to the request

external: if the referrer host is not en(.m)?.wikipedia.org
   

## Usage

1. The HQL commands can be used on similar large datasets, specifically those found in Wikipedia dumps - https://dumps.wikimedia.org/
2. This script was designed to answer all sorts of questions pertaining to big data.

## Contributors

* Devansh Sharma
* Rajkumar K
* Sailash R
* Aparna Sankarasetti
* Ashish Kumar
* Pooja Kumari


## Data Set used

* [Pageviews Filtered to Human Traffic](https://wikitech.wikimedia.org/wiki/Analytics/Data_Lake/Traffic/Pageviews)
    
* [Monthly Clickstream](https://meta.wikimedia.org/wiki/Research:Wikipedia_clickstream)

## License
This project includes the following license:
[MIT License](https://github.com/git/git-scm.com/blob/main/MIT-LICENSE.txt)
