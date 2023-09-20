# The New York Social Graph Project
## Objective
In this project I built a social network for New York's social elite by web scraping the [New York Social Diary](https://colab.research.google.com/corgiredirector?site=https%3A%2F%2Fweb.archive.org%2Fweb%2F20150913224145%2Fhttp%3A%2F%2Fwww.newyorksocialdiary.com%2F). The data forms a natural social graph for New York's social elite. To create the social newtrok for New York's social elite, I conducted the follwoing stages:
1. Web scraped the [New York Social Diary](https://colab.research.google.com/corgiredirector?site=https%3A%2F%2Fweb.archive.org%2Fweb%2F20150913224145%2Fhttp%3A%2F%2Fwww.newyorksocialdiary.com%2F) webpage using Beautiful Soup and API request.
2. Studied the structure of the pages in the archive and parsed all the captions that dated before December 2014
3. Used natural language processing capabalities of NLTK and regex to parse all the names in the captions
4. Build the social graph with the assumption that people in the same picture know each other thus belong to a social network. The network was designed using python's [NetworkX](https://colab.research.google.com/corgiredirector?site=https%3A%2F%2Fnetworkx.github.io%2F) library. The connection between each celebrity pair is constructed using an undirected weighted graph.
5. Using Networkx, this network build the social network and find the most popular socialites, most influential people and the most tightly connected pairs.

For a more comprehensive understanding of this project, please consult the complete Colab notebook of my project, accessible [here](https://github.com/hhaeri/The-New-York-Social-Graph/blob/main/social_network_graph.ipynb).
