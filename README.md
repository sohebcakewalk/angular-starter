# Quiz

- Where and how can you use JQuery with the SDK?
    - jQuery (crawler) aka Cheerio crawler downloads each URL using a plain HTTP request, parses the HTML content using Cheerio and then invokes the user-provided CheerioCrawlerOptions.handlePageFunction to extract page data using a jQuery-like interface to the parsed HTML DOM.
    - Since CheerioCrawler uses raw HTTP requests to download web pages, it is very fast and efficient on data bandwidth
- What is the main difference between Cheerio and JQuery?
    - Cheerio is a server-side version of the jQuery library. It does not require a browser but instead constructs a DOM from a HTML string. It then provides the user an API to work with that DOM.
    - jQuery runs in a browser and attaches directly to the browser's DOM. Where does cheerio get its HTML
    - Unlike jQuery, Cheerio doesn't have access to the browser’s DOM .         Instead, we need to load the source code of the webpage we want to crawl. Cheerio allows us to load HTML code as a string, and returns an instance that we can use just like jQuery.
- When would you use CheerioCrawler and what are its limitations?
    - Cheerio Scraper is ideal for scraping web pages that do not rely on client-side JavaScript to serve their content and can be up to 20 times faster than using a full-browser solution such as Puppeteer.
    - It does not employ a full-featured web browser such as Chromium or Firefox, so it will not be sufficient for web pages that render their content dynamically using client-side JavaScript
- What are the main classes for managing requests and when and why would you use one instead of another?
    - There are two main classes which are **RequestList** or **RequestQueue** which derived from **Request**
- How can you extract data from a page in Puppeteer without using JQuery?
- What is the default concurrency/parallelism the SDK uses?
