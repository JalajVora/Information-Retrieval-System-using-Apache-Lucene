# Information-Retrieval-System-using-Apache-Lucene-in-JAVA

This is a command-line based Inforamtion Retrieval System built in JAVA using Apache Lucene search library [^1].

+ Using Lucene, it parses and indexs Plain Text and HTML documents that a given folder and its subfolders contain. Also, all parsed files are listed.
+ English language is considered to Stem (e.g. using Porter Stemmer).
+ A search index is selected or a new one is created (if not available in the chosen directory).
+ User can choose the ranking model with keywords as; Vector Space Model (VS) or Okapi BM25 (OK).
+ A ranked list of relevant articles given a search query are printed. The output contains the 10 most relevant documents with their rank, relevance score, file name resp. title (if it is a HTML-file containing title information) and the path.
+ Multiple fields are concurrently searched (multifield search): not only the document’s text (body tag) are searched, but also its title.

To know more about what an individual JAVA files do, please refer the [documentation.](https://github.com/JalajVora/Information-Retrieval-System-using-Apache-Lucene/blob/master/docs/Programming_documentation.pdf)


[^1]: http://lucene.apache.org/java/
### _How to run the Program:_

**Step1:** Keep jar file in your desired location.

**Step2:** Make sure that you have created index directory and document directory which consist of sample files for indexing in desired location.

**Step3:** Open command line and change directory to the directory where jar file has been present.

**Step4:** Enter the command as:

`java -jar IR_P.jar [path to document folder] [path to index folder] [VS/OK] [query]`
	
**Step5:** Results will be displayed on the console.
