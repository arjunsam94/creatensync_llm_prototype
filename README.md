# Building an LLM prototype - CreateNSync

## Background
While more professionals are entering the creator economy, not all creators can rely on income from advertising and sponsorships since it requires significant high value followers. Affiliate marketing is a more viable path to revenue for many creators with smaller following considering lower barrier to entry for this channel. The tool aims to use LLM models to help creators find affiliate opportunities relevant to their content without much hassle.

## Problem
* Significant proportion of full-time and part-time creators earn < $10K annually. As a result, only less than 30% become full-time creators, making it a highly volatile profession.
* Without a significant following, brand sponsorships are hard to come by which leaves **affiliate partnerships** as a viable option for many creators.
* Means of connecting creators and relevant products for affiliate partnerships have largely remained unchanged, relying mostly on companies reaching out to creators rather than creators having more control over the process.

## Solution
A tool where content creators can just upload their content and automatically identify the most relevant products they can partner with for affiliate opportunities. The prototype of the platform currently includes:

* Audio transcription using whisper small model.
* Used zero-shot classification model (bart-large-mnli) to identify the relevant category of the transcribed text by comparing it against product categories scraped from ProductHunt, using BeautifulSoup.
* The top products by ratings from the relevant category are scraped to help creators find relevant affiliate opportunities from ProductHunt.

## Results
Pitched the prototype to judges from organizations like Google, Amazon, and Madrona Ventures and was recognized as the most creative among 10 projects presented that day. 

## Considerations
* The size and format of the content can significantly impact the user experience since these factors can significantly increase the time and cost to find good affiliate matches. It is important to beta test different content formats and sizes in stages before launching the finished product.
