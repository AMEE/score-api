Company Resource
================

The company resource relates to the amee environmental data for a given company, using a particular identifier, like a company registration number (`CRO`) or amee id (`AMEE`)

Get company
-----------

* `GET /api/companies/{company_id}` - Get data for a single company.  

### Query Parameters

`type` - the type of the company ID specified, (CRO|amee).  If no type is specified, defaults to amee.

* `CRO`  - company registration number
* `amee` - amee id


Sample Request
--------------

Making the following request for a company's score:

```shell
curl -u key:secret https://data.amee.com/api/companies/000662801
```

Sample Response
---------------


Will return the following json:

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




