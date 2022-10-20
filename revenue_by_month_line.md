## Revenue By Month

A line chart of revenue by month

### Specification

An API endpoint that returns JSON in the format:

``` 
    revenueByMonth = [
        {
            "id": "2018",
            "data": [
                {
                    "x": "January",
                    "y": 16569500,    
                },
                {
                    "x": "February",
                    "y": 16696585
                },
                ...
            ],
        },
        {   
            "id": "2019",
            "data": [
                {
                    "x": "January",
                    "y": 16569500,    
                },
            ],
            ...
        }
        ...
    ] 
```

This returns a list of objects where the key:
 * "id" denotes year in "YYYY" format. It should return the years from 2018 to the latest month running in the simulator.

Each object has a data value which is a list of objects where:
 * "x" denotes the month in the format "MMMM"
 * "y" is the sum of the `fare` column

