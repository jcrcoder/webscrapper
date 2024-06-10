# Web Scrapper project

## Description
This is a simple test that uses LLMs to extract data from a web scrape.  
*Based on https://github.com/redamarzouk/Scraping_Agent*

## Main components used
- Uses Firecrawl : Markdown version of site, no HTML code
- OpenAI
- Jina AI : Text-only version of site, not even MD
- Tiktoken : get


## Some notes
- Jina AI uses less tokens
- Jina AI returned less results when testing in TB/smartphones search (Firecrawl: 8 objects, JinaAI: 5 objects. Firecraw was 100% accurate)