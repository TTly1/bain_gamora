---
title: "Suchmaschinen und Discovery-Systeme"
date: 2021-12-17
---

In the last lecture of 2021, we used all our knowledge from the past lectures and (converted) file. The goal was to dive into the search engine and discovery systems of the VuFind software. 

After the recap of the last lecture, we had a small digression of JSON-API. I have learned that most API’s often deliver data in JSON format (just like XML, JSON is a text-based data format and can be viewed on browser). (I have tried to read more about it on the web, but I found it to be very technical - and did not understand the advantages and disadvantages fully). 

### Solr
Solr (Searching On Lucene w/ Replication) is an open-source-software that is the base (standard) for many search engine providers. The discovery-system of VuFind is also based on Solr. In order that the search is also effective, it is necessary to set a schema before the import of the file. So that the engine knows what kind of data (text, number, boolsch value etc.) and what field is in the file. 
It was interesting to see the difference between a database (SQL) search query and Solr (search index). While a database is more suitable for CRUD (Create, Reade, Update, Delete) of data, the Solr (search index) is used for retrieval of data. 

#### Solr Usability 
The interface of the Solr is a bit overwhelming. First time users are faced with many numbers and terms they may not understand. The icons however, can help users to understand the meaning. 
The search fields (input field) have an old design (very basic, however, the usability (the look and feel) has room for improvement. The search field is similar to a form, which forces the user to (depending on the screen) to scroll. Also, no required fields are marked. And last, the empty space of this page is too big. I would suggest dividing the input fields in more widgets, distributing it horizontally on the page. The tooltip when hovering on the parameters is very helpful, and increases the usability. 

### Hands-On Solr with VuFind
VuFind had already been installed, and with that also Solr. The Solr interface was accessible through the URL: ( http://localhost:8983/ ). The task given,  to search for the term “psychology” on VuFind and on Solr, and compare both outputs. The input on Solr is a bit harder, since users need to be aware, to not only enter the search term, but also “where to look for”. In our case: allfields:psychology. The results of both queries were the same, which makes sense, since both search engines are based on the same technology. The big difference however is the display of the results. While Solr displays the result in JSON format, the VuFind has a more clean and user-friendly view (an Online Public Access Catalogue (OPAC) view). It was also clear to see that the amount of data from Slor was bigger than what VuFind presented. This is because VuFind already filters the amount of data displayed. 

We also needed to import MARCXML files into VuFind. Because of the missing ID it also failed for me, so I participated passively. 

Overall, it was interesting for me to see how the output of a search query looked in the JSON format. 


