### Industrial Project Amazon Scrapper
Start project with: 
<ul>
<li>npm install</li>
<li>npm i</li>
<li>npm i -g amazon-buddy</li>
</ul>

### Purpose of this amazon scrapper
As websites scrapping is completly legal, without touching  retrieving any sensitive data such as credentials, \
logins  and so on, a website scrapping details has it's purpose when product details from specific websites are needed. \

Let's suppose we need a JSON file with all details related to an amazon product. \
This kind of JSON file is needed for example for Industrial Project CRUD API Firebase, and further to the website developed for this whole project. \

Let's start with understanding amazon website and URLs. 
1. Open Google and write next: "Amazon SAMSUNG 49-Inch CHG90 144Hz Curved Gaming Monitor (LC49HG90DMNXZA) – Super Ultrawide Screen QLED Computer Monitor, 3840 x 1080p Resolution, 1ms Response, FreeSync 2 with HDR,Black" \
2. This is a simple search for Amazon website with a product name - a Smasung Ultrawide Screen QLED \
3. Now, open the first link Google has returned. \
4. In my case, the URL is next one: 
```
https://www.amazon.com/Samsung-49-Inch-Curved-Monitor-LC49HG90DMNXZA/dp/**B072C7TNC5**"
```
The asin for this product can be found in the above URL, rigth after/dp/. 
In the example above this is:
```
B072C7TNC5
```
### Run the scrapper and obtain a JSON as a response, containing B072C7TNC5 product details
1. In Visual Code Terminal, run:
```
amazon-buddy products -k 'SAMSUNG 49-Inch CHG90 144Hz Curved Gaming Monitor (LC49HG90DMNXZA) - Super Ultrawide Screen QLED Computer Monitor, 3840 x 1080p Resolution, 1ms Response, FreeSync 2 with HDR,Black' -n 1 --filetype json
```
In my case next file was saved: products(SAMSUNG 49-Inch CHG90 144Hz Curved Gaming Monitor (LC49HG90DMNXZA) – Super Ultrawide Screen QLED Computer Monitor, 3840 x 1080p Resolution, 1ms Response, FreeSync 2 with HDR,Black)_1712770654253.json

OR RUN
```
amazon-buddy asin B072C7TNC5 -n 1 --filetype json
```
In my case next file was saved: asin(B072C7TNC5)_1712771589712.json


### What can we do with this website scrapper?
We obtain real data for any product desired from Amazon in this case (can be mapped to any website) and has / have a JSON format.

### How does product details retried look like?
I will explain further next JSON file, retrieved earlier:
```
products(SAMSUNG 49-Inch CHG90 144Hz Curved Gaming Monitor (LC49HG90DMNXZA) – Super Ultrawide Screen QLED Computer Monitor, 3840 x 1080p Resolution, 1ms Response, FreeSync 2 with HDR,Black)_1712770654253
```



### This scrapper is inspired from GitHub amazon-scrappers, it does have some updateds made by team group projet members but this scrapper is inspired from GIT.
