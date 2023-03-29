# WebScraping
this Repository contains  python web Scraping projects.

In this article, we are going to see how we can scrape the amazon customer review using Beautiful Soup in Python.

Module needed
bs4: Beautiful Soup(bs4) is a Python library for pulling data out of HTML and XML files. This module does not come built-in with Python. To install this type the below command in the terminal.
pip install bs4

requests: Request allows you to send HTTP/1.1 requests extremely easily. This module also does not come built-in with Python. To install this type the below command in the terminal.
pip install requests

To begin with web scraping, we first have to do some setup. Import all the required modules. Get the cookies data for making the request to amazon, without this you can not able to scrape. Create a header that contains your request cookies, without cookies you can not scrape amazon data it always shows some error. This website will provide you, specific user agent.


Pass the URL in the getdata() function(User Defined Function) to that will request to a URL, it returns a response. We are using get method to retrieve information from the given server using a given URL.

Syntax: 

requests.get(url, args)

Convert that data into HTML code and then Parse the HTML content using bs4.

Syntax: soup = BeautifulSoup(r.content, ‘html5lib’)

Parameters:

r.content : It is the raw HTML content.
html.parser : Specifying the HTML parser we want to use.
