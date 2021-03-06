# Welcome to Beacon - Registry

This is a Proof of Concept to show how [Beacon's Web Pages](https://beacon-network.org/#/), can be enriched by [DataCatalog schema](http://schema.org/DataCatalog) and made it easy to mantain an updated registry of existing beacons and it's datasets.

## Requirements

For this Proof of concept to work you will need:
1. Homebrew installed. [Installation](https://brew.sh/)
2. Python 3 with virtual environment installed. [Installation](https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-local-programming-environment-on-macos)
3. Scrapy installed. [Documentation](https://doc.scrapy.org/en/latest/intro/tutorial.html)
4. Install Extruct. [Installation](https://github.com/scrapinghub/extruct)
5. Install a Web Server as [XAMPP](https://www.apachefriends.org/index.html) to host modified beacon's pages.
6. Test your Web Pages Modifications [Google Schema Validator](https://search.google.com/structured-data/testing-tool)

## Proposed Schema from schema.org (DataCatalog)
```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Beacon Sample Structure</title>
  </head>
  <body>
    <div vocab="http://Schema.org/" typeof="DataCatalog" class="main-container">
      <h1 property="name">Beacon's Name</h1>
      <span property="description">Here you put the Beacon's despcription</span>
      <select typeof="DataSet" property="dataset">
          <option property="name" value="genes1">Genes1</option>
          <option property="name" value="genes2">Genes2</option>
          <option property="name" value="genes3">Genes3</option>
          <option property="name" value="genes4">Genes4</option>
      </select>
      <span property="version">API version 0.0.0</span>
    </div>
  </body>
</html>
```
## Sample Beacon GA4GH Beacon with DataCatalog Schema
![Sample of GA4GH Beacon with ](http://gdurl.com/SI21)

## Process
This image summarises the process of this Proof Of Concept

![Image of Beacon - Registry Project](http://gdurl.com/MJFd)


### Support or Contact

For futher information [contact](mailto:guillermo.calderon@elixir-europe.org) or @guicalman.
