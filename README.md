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
* Zero-shot classification model (bart-large-mnli) to identify the relevant category of the transcribed text by comparing it against product categories scraped from ProductHunt, using BeautifulSoup.
* Top products by ratings from the relevant category scraped from ProductHunt to help creators find relevant affiliate opportunities.

## Results
Pitched the prototype to judges from organizations like Google, Amazon, and Madrona Ventures and was recognized as the most creative among 10 projects presented that day. 

## Observations
* The size and format of the content significantly impacted the user experience since these factors increased the time to find good affiliate matches.
* Filtering the search to products matching the relevant category proved to be a challenge with a search engine, since it returned irrelevant ads even with search operators. It might be better to expand product searches outside ProductHunt through partnership with marketplaces like ConvertKit or Impact for affiliate opportunities.
