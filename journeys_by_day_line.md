## Journeys By Day

A line chart of the count of the journeys by day

### Specification

An API endpoint which of this format:

`http://sub-domain.domain/path/<YYYY-MM-DD>` 

where `<YYYY-MM-DD>` is a variable representing a year and month.

Eg: `http://sub-domain.domain/path/2021-10-30`

```
    journeysByHour = [
        {
            "id": "30th October 2021",
            "data": [
                {
                    "x":"00",
                    "y":5187
                },
                {
                    "x":"01",
                    "y":4302
                },
                ...
            ]
        },
        {
            "id": "29th October 2021",
            "data": [
                {
                    "x": "00",
                    "y": 5630
                },
                ...
            ]
        },
        {
            "id": "23rd October 2021",
            "data": [
                {
                    "x": "0",
                    "y": 8527
                },
                ...
            ]
        }
    ]
```
This returns a list of objects where the key:
 * "id" denotes the day in "Do MMMM YYYY" format.
 
 It should have the day from the URL, the previous day,
 and the same day previous week. Eg
 `2021-10-30` should produce these ids:
 * 30th October 2021
 * 29th October 2021
 * 23rd October 2021

Each object has a data value which is a list of objects where:
 * "x" denotes the hour in the format "HH"
 * "y" is the count of the journeys



