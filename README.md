# Text Summarization
## Introduction
There is an enormous amount of textual material, and it is only growing every single day.
Think of the internet, comprised of web pages, news articles, status updates, blogs and so much more. The data is unstructured and the best that we can do to navigate it is to use search and skim the results. There is a great need to reduce much of this text data to shorter, focused summaries that capture the salient details, both so we can navigate it more effectively as well as check whether the larger documents contain the information that we are looking for.
Text summarization is the process of creating a short and coherent version of a longer document.
Humans are generally good at this type of task as it involves first understanding the meaning of the source document and then distilling the meaning and capturing salient details in the new description. However, it is not enough to just generate words and phrases that capture the gist of the source document. The summary should be accurate and should read fluently as a new standalone document. There are many reasons and uses for a summary of a larger document.
One example that might come readily to mind is to create a concise summary of a long news article, but there are many more cases of text summaries that we may come across every day. For example:
- headlines (from around the world)
- outlines (notes for students)
- minutes (of a meeting)
- previews (of movies)
- synopses (soap opera listings)
- reviews (of a book, CD, movie, etc.)
- biography (resumes, obituaries)
- bulletins (weather forecasts/stock market reports)
- sound bites (politicians on a current issue)

## Implementation
The text was first cleaned and formatted. It was then tokenized and vectorized after which, a similarity matrix was built which measured the similarities between the sentences in the article by taking their cosine difference. Google's Page Rank algorithm was run over this similarity matrix, and the top n sentences with the highest scores were picked to form the summary.

## Input and Output
* Input: Link to any wikipedia page and the size of the required summary 
* Output: Summary of n sentences
