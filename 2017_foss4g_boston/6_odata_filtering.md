# 6] OData filtering

For querying the SensorThings API adheres to the <a href="http://www.odata.org/documentation/">OASIS OData 4.0 standard</a>. In this exercise
we will explore the various OData options.

For sample urls see <a href="https://github.com/gost/docs/blob/master/gost_queryoptions.md">gost_queryoptions.md</a> (for selection, ordering, pagination options) and <a href="https://github.com/gost/docs/blob/master/gost_filtering.md">gost_filtering.md</a> (for logical, arithmic, grouping, string, date and geospatial functions).

A sample filter requests looks like this:

Retrieve all datastreams with name equals to 'test1'

```
$ curl http://localhost:8080/v1.0/Datastreams?$filter=name eq 'test1'
```

The part after the $filter contains the OData query

## Exercise Logical filter

Construct and test a query to get all observations with result value bigger or equal than 1.

## Exercise String filter

Construct and test a query to get all datastreams where name starts with 'Number'

## Geospatial

Construct and test a query to get all locations in Boston (-72 42, -72 43, -70 43, -70 42, -72 42) using geo.intersects.

## Date

Construct and test a query to get all observations where phenomenonTime is in month August


Continue to <a href = "7_bonus_exercise.md">7) Bonus exercise</a>
