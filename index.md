## This is Harsh's page. 

### About Myself
I'm a MS by Research student at Robotics Research Center, IIIT-Hyderabad. I work on Non Linear Controls and it's applications in autonomous vehicles. I'm also really interested in NLP and Reinforement Learning. Apart from this stuff, you can mostly find me watching movies or creating my own music with my Guitar/Keyboard. 

### Publications
- "Adaptive-robust controller for a class of systems with time-varying input delay and state-dependent uncertainty". Spandan Roy, Harsh Shukla. Control Strategy for Time-Delay Systems: Part I: Concepts and Theories. 
- "Robust Adaptive Control of Steer-by-Wire Systems under Unknown State-dependent Uncertainties". Harsh Shukla, Spandan Roy and Saksham Gupta. Submitted for review in International Journal of Adaptive Control and Signal Processing. 

### Selected Projects 

#### Wikipedia-Search-Engine 
Developed a search engine over the 75GB Wikipedia dump. Both simple and multi field queries have been implemented. The search returns a ranked list of articles in real time.

##### Indexing:

- Parsing: SAX Parser is used to parse the XML corpus.
- Casefolding: Converting Upper Case to Lower Case.
- Tokenisation: It is done using regex.
- Stop Word Removal: Stop words are removed by referring to the stop word list returned by nltk.
- Stemming: A python library PyStemmer is used for this purpose.
- Creating various index files with word to field postings.
- Multi-way External sorting on the index files to create field based files along with their respective offsets.

##### Searching:
- The query given is parsed, processed and given to the respective query handler(simple or field).
- One by one word is searched in vocabulary and the file number is noted.
- The respective field files are opened and the document ids along with the frequencies are noted.
- The documents are ranked on the basis of TF-IDF scores.
- The title of the documents are extracted using title.txt
