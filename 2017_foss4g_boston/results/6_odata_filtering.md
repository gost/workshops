- Exercise: Construct and test a query to get all observations with result value bigger or equal than 1.

Answer: http://localhost:8080/v1.0/Observations?$filter=result ge 1

- Exercise: Construct and test a query to get all datastreams where name starts with 'Number'

Answer: http://localhost:8080/v1.0/Datastreams?$filter=startswith(name,'Number')

- Exercise: Construct and test a query to get all locations in Boston (-72 42, -72 43, -70 43, -70 42, -72 42) using geo.intersects

Answer: http://localhost:8080/v1.0/Locations?$filter=geo.intersects(location, geography'POLYGON ((-72 42, -72 43, -70 43, -70 42, -72 42))')

- Exercise: Construct and test a query to get all observations where phenomenonTime is in month August

Answer: http://localhost:8080/v1.0/Observations?$filter=month(phenomenonTime) eq 8
