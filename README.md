# Web Scrapper project

## Things required to run
- run `pip install -r requirements.txt`
- create python venv
- create .env file with proper keys
1) FIRECRAWL_API_KEY=fc-xxxx
2) OPENAI_API_KEY=sk-xxxxxx

## Description
This is a simple test that uses LLMs to extract data from a web scrape.  
*Based on https://github.com/redamarzouk/Scraping_Agent*
*Also on https://github.com/trancethehuman/ai-workshop-code/blob/main/Web_scraping_for_LLM_in_2024.ipynb*

## YT tutorials

Based on Reda Marzouk tutorial for data scraping 
https://www.youtube.com/watch?v=ncnm3P2Tl28&ab_channel=RedaMarzouk

https://youtu.be/QxHE4af5BQE?si=_QdyuHWlRG6vZ0fE (Jina AI and Tiktoken)

## Main components used
- Uses Firecrawl : Markdown version of site, no HTML code, MD tags
- OpenAI : 3.5 worked just as good at parsing. Can save $ by using older model
- Jina AI : Text-only version of site returned, not even MD
- Tiktoken : tokenize content to calculate OpenAI costs


## Some observations
- Jina AI uses less tokens than Firecrawl
- Jina AI returned less results when testing in Techbargains/smartphones search (Firecrawl: 8 objects, JinaAI: 5 objects. Firecraw was 100% accurate)
