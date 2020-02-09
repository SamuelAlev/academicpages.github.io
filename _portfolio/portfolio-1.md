---
title: "INAMI API"
excerpt: "API on top of the form used by the Belgian INAMI eHealth service.<br/><img src='/images/inami.png'>"
collection: portfolio
---

Since their is no public INAMI API but just a [web form](https://ondpanon.riziv.fgov.be/SilverPages/) available.

I did a multi-process web scrapper on the website which is updating the data every month (without any impact on their website) and expose the data as an API.
The API is hosted on [Heroku Free Tier](https://heroku.com/) and use [MongoDB free mLab](https://www.mongodb.com/) as storage.
The web scrapper is made using [NodeJS](https://nodejs.org/) and [Puppeteer](https://github.com/puppeteer/puppeteer).

The form is really bad as:
1. No API was available, always needed to pass by the form;
2. The form was slow (search was really slow and there is no cache available)

This API have:
1. Good speed with the help of caching (with Redis);
2. [Documentation](https://inami.samalev.be/docs/v1/)
