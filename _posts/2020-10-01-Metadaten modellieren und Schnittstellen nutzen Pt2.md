---
title: "Metadaten modellieren und Schnittstellen nutzen (2/2)"
date: 2021-12-03
---

The second lecture on the modeling metadata and interfaces is to transform the metadata with OpenRefine. 

### OpenRefine
[OpenRefine](https://openrefine.org/) is an open-source desktop application for data cleanup and transformation to other formats. It is similar to spreadsheet (excel) applications and can handle spreadsheet file formats such as CSV, but it behaves more like a database. Apart from cleaning, and transformation, it also allows enrichment of external data (a special function of OpenRefine). 


OpenRefine is not a cloud base software and needs to be locally installed (meaning all data stays in the computer) but it is usually operated through the browser.
The data quality is not always as from the standards expected (this is the reason why we used OpenRefine). 

According to a survey OpenRefine is mostly used by librarians, but also other data-focused subjects such as data scientists, data journalists, etc. are users of OpenRefine. This shows that the area of application is very broad. The survey has also shown that most of the users use it for the “normalization” of data (clean-up, e.g. correction of typos), but also in the transformation of the data (from one format to another).

OpenRefine can also be used in combination with MarcEdit for analysis and transformation purposes. 

After the theoretical introduction, we had our hands-on experience. First as mentioned, install OpenRefine in our virtual box (by using as usual the terminal).  
After the installation, we had to import CSV data (which was given to use) and check the data inconsistency. The first step was to group the language facet (understanding how many different languages or spelling we had in our data). Since English was written in two different ways (EN with over 800 entries and English with over 100), we had to standardize the language English first. Since there were also other languages FR (French) and ES (Spanish), we thought it would be best to have all languages which were English in EN. 

The split-multi-valued cells (facet - author), help to standardize how authors are separated by. 

#### Transformation 
After the introduction of a few standardizing features, we had to convert our file, which was in a CSV format to MARCXML. The first step was to create a sort of template (GREL template language). The creation of such a template requires basic knowledge of script language and is not as easy as the previous steps (Templating Export). I did not understand why we had to create such a template. 

Last but not least, validation is needed, and this was done with the program: xmllinit. 

### OpenRefine Usability:
The design reminded me of an old Google application. But also like MarcEdit, it is a very straightforward application. I can however imagine that there may be confusion when the user’s goal is to import data, but only finds import projects or create projects at first sight. However, once the association was made, the preview function is great to prevent errors (e.g. uploading the wrong file). Therefore, it was very well solved! Also the feedback function, after the execution of a command (changing the languages from English to EN) is very helpful and increases the usability / UX of the software. 

The facet widget on the left is very small when dealing with large data, but it is very easy to use since the user has the possibility to sort the list, and check by only one look at the inconsistency of the data and easily edit the data. The cluster function is a great usability function, facilitating the usage and giving the user proposals to choose from. 
