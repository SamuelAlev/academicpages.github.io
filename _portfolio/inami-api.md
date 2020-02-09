---
title: "INAMI API"
excerpt: "<img src='/images/inami.png'><br/>API on top of the form used by the Belgian INAMI eHealth service."
collection: portfolio
---

Since there is no public INAMI API but a [web form](https://ondpanon.riziv.fgov.be/SilverPages/) available on the INAMI website.

I did a multi-process web scrapper on the website which is updating the data every month (without any impact on their website) and expose the data as an API ([the datas are free to use](https://www.riziv.fgov.be/fr/Pages/informations-legales.aspx)).  
The API is hosted on [Heroku Free Tier](https://heroku.com/) and use [MongoDB free mLab](https://mlab.com/) as storage.  
The web scrapper is made using [NodeJS](https://nodejs.org/) and [Puppeteer](https://github.com/puppeteer/puppeteer).  
  
The documentation is present [here](https://inami.samalev.be/docs/v1/)
