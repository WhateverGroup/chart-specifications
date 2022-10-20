## Journeys By Day

A line chart of the count of the journeys by day

### Specification

An API endpoint which of this format:

`http://sub-domain.domain/path/<YYYY-MM>` 

where `<YYYY-MM>` is a variable representing a year and month.

Eg: `http://sub-domain.domain/path/2021-10`

```
    journeysByHour = [
        {
            "id": "September 2021",
            "data": [
                {
                    "x":"01",
                    "y":88185
                },
                {
                    "x":"02",
                    "y":93100
                },
                ...
            ]
        },
        {
            "id": "October 2021",
            "data": [
                {
                    "x": "01",
                    "y": 95630
                },
                ...
            ]
        },
        {
            "id": "October 2020",
            "data": [
                {
                    "x": "01",
                    "y": 88527
                },
                ...
            ]
        }
    ]
```
This returns a list of objects where the key:
 * "id" denotes the month in "MMMM YYYY" format.
 
 It should have the month from the URL, the previous month,
 and the same month previous year. Eg
 `2021-10` should produce these ids:
 * October 2021
 * Septemeber 2021
 * October 2020

Each object has a data value which is a list of objects where:
 * "x" denotes the day in the format "DD"
 * "y" is the count of the journeys



