## Total Revenue
A sum of the total revenue for a day

### Specification

An API endpoint which of this format:

`http://sub-domain.domain/path/<YYYY-MM-DD>` 

where `<YYYY-MM-DD>` is a variable representing a year, month and day.

Eg: `http://sub-domain.domain/path/2021-10`

The response from the endpoint should be:

```
    { "totalRevenue" : 1581445 }
```

where the figure represents the sum of the `fare` of the number of journeys for the day supplied in the URL.