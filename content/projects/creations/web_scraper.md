{
  "title": "Web Data Extraction",
  "date": "2024-01-05T12:41:05-05:00",
  "link": "https://github.com/sarapiscitelli/web-data-extraction",
  "image": "/img/web_extraction_1.png",
  "description": "A simple web crawler and scraper has been developed to extract data from websites. The crawler operates on Scrapy, while the scraper utilizes BeautifulSoup. At present, the scraper is configured to extract structured data specifically from the Trustpilot.com website. For other sites, the scraper is designed to return unstructured text data",
  "tags": ["Scrapy", "crawling","web", "Python"],
  "fact": "",
  "featured":true
}

A simple web crawler and scraper has been developed to extract data from websites. The crawler operates on Scrapy, while the scraper utilizes BeautifulSoup. At present, the scraper is configured to extract structured data specifically from the Trustpilot.com website. For other sites, the scraper is designed to return unstructured text data.  

#### Current features
- [✅] **extract_from_url API**:
    - This API enables text extraction from a list of any website URL, utilizing the [trafilatura](https://trafilatura.readthedocs.io/en/latest/usage-python.html) library for text content extraction.
    - It offers the ability to recursively navigate within a webpage, staying within the same domain. Users can specify this using the max_next_pages parameter (where 0 denotes only the current URL, and a higher number allows navigation through multiple pages)

- [✅] **extract_from_trustpilot_url API**:
  - This feature focuses on extracting formatted content from a specific organization's page on [trustpilot](https://www.trustpilot.com)
  - It also includes functionality to navigate through subsequent pages to gather all reviews, controlled by the max_next_pages parameter.
