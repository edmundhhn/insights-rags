# insights-rags

## Background
__Imagine you are an employee at a large retail company.__ Every day there are millions of articles which could be relevant to your job function, whether this be news, insights or research papers. The problem? there is simply too much public information out there to sift through one by one, with so much work to get done, who has the time for that? The result? A lot of valuable (and free!) information is not leveraged in everyday workflows. Take McKinsey's insights pieces for example! Excellent free information but heavily underleveraged.

Our solution to this is to develop a RAG based system which can collect these articles and use it to generate a digestable newsletter that any office worker can read at the beginning of their day. Because of the power of Generative AI, these can be personalized and tuned to maximize relevance and impact to the reader. 

## Project Workflow
1. Identify relevant source articles, build a scraper that can store them into directory
2. Use an embedding method e.g. AWS Bedrock to store in a vector database e.g. ChromaDB for querying
3. Set up multiple RAG queries to write entire newsletter segments based on the most impactful and relevant information from the database
4. Use responses to populate a bite sized news letter format with links to the original sources if you wish to read more
