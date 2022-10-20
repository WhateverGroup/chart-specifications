## Total Journeys Count
A count of the total journeys for a month

### Specification

An API endpoint which of this format:

`http://sub-domain.domain/path/<YYYY-MM-DD>` 

where `<YYYY-MM-DD>` is a variable representing a year, month and day.

Eg: `http://sub-domain.domain/path/2021-10-30`

The response from the endpoint should be:

```
    { "totalJourneys" : 119589 }
```

where the figure represents the count of the number of journeys for the day supplied in the URL.