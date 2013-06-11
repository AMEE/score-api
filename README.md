Using the amee Score API
========================

Looking to use amee's score API? 

Everything you need to start is listed right here, including sample code and detailed documentation

Where to start
--------------

1. The first thing you'll need are some API credentials to sign requests with. You can get those from the [API page on amee.com](https://www.amee.com/pages/api)
2. Once you have credentials, see how to make a sample request using your credentials, and see a sample response.
3. Join the [Score API group](https://groups.google.com/forum/?fromgroups&hl=en#!forum/amee-score-api) to talk to others using the APIs and give us feedback.

Making a sample request
------------------------

Once you have credentials, you can make a sample request to the amee Score resource like so:

```shell
curl -u key:secret https://data.amee.com/api/companies/000662801
```

You should receive a json response looking something like this:

```json
{"company": {
    "amee_company_id": "000662801",
    "name": "Amee Uk Ltd",
    "amee_industry_score": 98,
    "amee_score_status": "updated",
    "annual_sales_local": 1999099,
    "city": "LondoN",
    "country_code": "GB",
    "currency_code": "GBP",
    "emissions_scope1_tco2e": null,
    "emissions_scope2_tco2e": null,
    "emissions_status": "updated",
    "emissions_total_tco2e": 984156,
    "employees_total": null,
    "uk_sic_2007": 62012,
    "national_identification_number": "06630234",
    "postcode": "EC1Y 2BJ",
    "province_name": "London",
    "street_address_1": "4th FlooR",
    "street_address_2": "70-74 City RoaD",
    "street_address_3": null,
    "street_address_4": null,
    "sustainability_report_url": null,
    "sustainability_report_year": 2013,
    "total_assets_local": 640291,
    "waste_hazardous_kg": 123000,
    "waste_non_hazardous_kg": 312000,
    "waste_status": "updated",
    "water_status": "updated",
    "water_withdrawn_l": 324000
}}
```


Authentication
--------------

All requests are sent over SSL, and use HTTP Basic Authentication with your user credentials. You can get those from the [API page on amee.com](https://www.amee.com/pages/api)


API Documentation
-----------------

There are currently two resources available on the public Score API:

* [Company](https://github.com/AMEE/score-api/blob/rails_api_v2/sections/company.md) - for returning the information for a given company


#### APIs under development

Over the coming weeks and months, we'll be exposing further resources to use, and fleshing out existing ones with new methods.  

* Company - fetching full information about companies, and sending updates to the data
* Search - exposing the search visible on http://amee.com in machine readable form


Help us make it better
----------------------

Please tell us how we can make the APIs better. If you have a specific feature request or if you found a bug, or the docs aren't clear, please [file an issue](https://github.com/AMEE/score-api/issues). Also, feel free to fork these docs and send a pull request with improvements!

To talk with us and other developers about the API, subscribe to the [amee developer mailing list](https://groups.google.com/forum/?fromgroups&hl=en#!forum/amee-score-api).
