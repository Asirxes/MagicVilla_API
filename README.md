# MagicVilla

A project based on creating standard RESTful APIs using .NET 7.

To use the project, download it, open it in visual studio and run it. After enabling, swagger should be enabled in the browser where you can test APIs endpoints. It is also possible to use localhost directly or after running appliacation use postman and try following:

GET https://localhost:7076/api/villaapi

GET https://localhost:7076/api/villaapi/{id}

POST https://localhost:7076/api/villaapi with body "{
    "name" : "new villa 4444",
    "occupancy" : 4,
    "sqft" : 300
}" for example

PUT https://localhost:7076/api/villaapi/{id} with body "{
    "id":3,
    "name":"new villa 333",
    "occupancy":4,
    "sqft":400
}" for example

PATCH https://localhost:7076/api/villaapi/{id} with body "[{
    "path":"/name",
    "op":"replace",
    "value":"new villa"
}]" for example

DELETE https://localhost:7076/api/villaapi/{id}

Make sure to fill id parameter, that app is running and when posting, puting and patching select body raw with json format.

Database is managed by sqlServer and in project Entity Framewrok is used to manipulate the data.

Registering informations to text file is implemented thanks to Serilog.
