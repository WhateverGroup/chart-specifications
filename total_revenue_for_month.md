## Total Revenue
A sum of the total revenue for a month

### Specification

An API endpoint which of this format:

`http://sub-domain.domain/path/<YYYY-MM>` 

where `<YYYY-MM>` is a variable representing a year and month.

Eg: `http://sub-domain.domain/path/2021-10`

The response from the endpoint should be:

```
    { "totalRevenue" : 46442526 }
```

where the figure represents the sum of the `fare` of the number of journeys for the month supplied in the URL.