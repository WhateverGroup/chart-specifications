## Revenue By Day

A calendar chart of the revenue by day.

### Specification

An API endpoint which returns a JSON object in the format:

```
    revenueByDay: [
        {
            day: "2018-01-01",
            value: 435386.86000000447
        },
        ...
    ]

```

The value field is the sum of the `fare` column for that particular day. The day field is a date in the format "YYYY-MM-DD".

The day should start on `2018-01-01` and include all days up
until the previous day of when the simulator is running.

