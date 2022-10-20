## Unique Riders
A count of unique riders for a month

### Specification

An API endpoint which of this format:

`http://sub-domain.domain/path/<YYYY-MM>` 

where `<YYYY-MM>` is a variable representing a year and month.

Eg: `http://sub-domain.domain/path/2021-10`

The response from the endpoint should be:

```
    { "uniqueRiders" : 3361175 }
```

where the figure represents the distinct count of user ids for the month supplied in the URL.