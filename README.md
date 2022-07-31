(Created this project and document using various websites and resources)

RAHUL SINGH THAKUR

NLP ACTIVITY

TEXT SUMMARIZATION

Text Summarization is an unsupervised learning method of a text span that conveys
important information of the original text while being significantly shorter. The
state-of-the-art methods are based on neural networks of different architectures as well as
pre-trained language models or word embeddings.
An example of Text summarization problem is news article summarization, which
attempts to automatically produce an abstract from a given article. Sometimes one might
be interested in generating a summary from a single source article, while others can use
multiple source articles (for example, a cluster of articles on the same topic). This
problem is called multi-document summarization. A related application is summarizing
news articles. Imagine a system, which automatically pulls together news articles on a
given topic (from the web), and concisely represents the latest news as a summary. An
example for this is App called inShorts, which summarizes news articles into 60 words.
Extractive summarization.

This type of summarization identifies relevant subset sentences from the input text and
uses them verbatim while still maintaining the original context of the input text.

Why Text summarization is important
The important uses of text summarization are,
● · Can get maximum information by spending minimum time from unstructured
textual data.
●●
· To enhance the readability of the documents.
●●
· Can eliminate redundant, insignificant text and provide required information
●●
· Accelerates the process of researching for information.

Tokenization & Data clean up

Import the stop words from NLTK toolkit and punctuations from strings library.
Stop words are a set of commonly used words in any language. For example, in English,
“the”, “is” and “and”, would easily qualify as stop words. In NLP and text mining
applications, stop words are used to eliminate unimportant words, allowing applications
to focus on the important words instead.
Creating the frequency table
Word tokenize the entire text. We have to create the dictionary with key as words and
value as number of times word is repeated.
Then divide the number of occurrences of all the words by the frequency of the most
occurring word, as shown below:
Tokenizing the article into sentences
To split the article_content into a set of sentences, we’ll use the built-in method from the
nltk library.
Finding the weighted frequencies of the sentences
To evaluate the score for every sentence in the text, we’ll be analysing the frequency of
occurrence of each term. In this case, we’ll be scoring each sentence by its words; that is,
adding the frequency of each important word found in the sentence.
Creation of summary
Using nalargest library get the top 30% weighted sentences. And later on join it to get the
final summarized text.
##END OF PART 1


Question Answering System


Question answering (QA) is a computer science discipline within the fields of
information retrieval and natural language processing (NLP), which is concerned with
building systems that automatically answer questions posed by humans in a natural
language.
A question answering implementation, usually a computer program, may construct its
answers by querying a structured database of knowledge or information, usually a
knowledge base. More commonly, question answering systems can pull answers from an
unstructured collection of natural language documents.
Some examples of natural language document collections used for question answering
systems include:
● a local collection of reference texts
● internal organization documents and web pages
● compiled newswire reports
● a set of Wikipedia pages
● a subset of World Wide Web pages
● Question answering research attempts to deal with a wide range of question types
including: fact, list, definition, How, Why, hypothetical, semantically constrained,
and cross-lingual questions.
Closed-domain question answering deals with questions under a specific domain (for
example, medicine or automotive maintenance), and can exploit domain-specific
knowledge frequently formalized in ontologies. Alternatively, closed-domain might refer
to a situation where only a limited type of questions are accepted, such as questions
asking for descriptive rather than procedural information. Question answering systems in
the context of machine reading applications have also been constructed in the medical
domain, for instance related to Alzheimer's disease.[2]
Open-domain question answering deals with questions about nearly anything, and can
only rely on general ontologies and world knowledge. On the other hand, these systems
usually have much more data available from which to extract the answer.
Explanation of what was done:-
Step1: Define different types of question patterns using regular expressions.
Step2: Tokenize into words and perform POS tagging to extract the subject for questions
starting with Where, who, what
and spilt the question into entities for questions starting with when.
Step3: Search in Wikipedia with extracted subject.
Step4: Search through the sentences for relevant answers using object and regular
expressions.
Step5: Return the most relevant answer to the user as result.
## END OF PART 2
