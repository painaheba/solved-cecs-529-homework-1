Download Link: https://assignmentchef.com/product/solved-cecs-529-homework-1
<br>



<ol>

 <li>Download the le NaiveIndex.java from BeachBoard’s Homework section. This le builds a simple boolean document-term matrix over a directory of .txt les. For this problem, you will extend the functionality in NaiveIndex to support a very simple information retrieval system. Follow these steps:</li>

</ol>

<ul>

 <li>Create a new Java project in your favorite IDE and add NaiveIndex.java to the project.</li>

 <li>Download the le MobyDick10Chapters.zip from BeachBoard. This le contains the rst 10 chapters of Herman Melville’s Moby Dick, each chapter separated into its own .txt le. Extract the ZIP le to the root of your project’s directory.</li>

 <li>Run NaiveIndex.java. The program should output a large matrix of 1’s and 0’s as a termdocument index. Make sure you understand the output and what it means.</li>

 <li>Modify the main method of NaiveIndex to build a simple search engine application:

  <ol>

   <li>Remove the call to index.printResults().</li>

   <li>Write a loop that continually scans a word from the user, until they enter the word quit .After scanning a word, print a list of indexed documents that contain the user’s term by walking through the mIndex member of the index variable in main. You will need to use a binary search to get the column number of the user’s term (see Java documentation for Arrays.binarySearch()) from the mTermArray variable. Then use a loop to walk through each entry in the corresponding column in mIndex, and if you nd a true at that matrix position, print out the corresponding document ID (since that document contains the requested term).</li>

   <li>Program this loop intelligently using good programming practices. Do not, for example, assume that there are only 10 documents; write your loop in terms of the array’s arbitrary length, whatever that may be.</li>

  </ol></li>

</ul>

<ul>

 <li>Example behavior: (user input in italics)</li>

</ul>

Enter a term to search for:    whale These documents contain that term: chapter1.txt chapter2.txt chapter3.txt chapter7.txt chapter9.txt

Enter a term to search for:    captain These documents contain that term: chapter1.txt chapter7.txt chapter8.txt chapter9.txt

Enter a term to search for:               quit

Bye!

<ul>

 <li>You should only modify the main method of the program and nothing else.</li>

</ul>

1