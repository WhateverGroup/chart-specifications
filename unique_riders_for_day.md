## Unique Riders
A count of unique riders for a day

### Specification

An API endpoint which of this format:

`http://sub-domain.domain/path/<YYYY-MM-DD>` 

where `<YYYY-MM-DD>` is a variable representing a year, month and day.

Eg: `http://sub-domain.domain/path/2021-10-30`

The response from the endpoint should be:

```
    { "uniqueRiders" : 71753 }
```

where the figure represents the distinct count of user ids for the day supplied in the URL.