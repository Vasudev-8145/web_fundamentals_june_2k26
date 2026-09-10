### API 
---
```Application programming interface that enables communication bw different applications```


### Webfundamentals
---

## client server architeture
    ```client sends an http request to server, server process the http request and send back http response ```

### http_methods
---
`GET` => fetch all resources  
`POST` => create an new resource  
`PUT` => update a resource  
`PATCH` => UPDATE a resource (partial update)  
`DELETE` => delete a resource  


### http_request_format
---

`url`  
`http_method`  
`Authorization`  
`body`  

### sample api end point
---

```
Employee

id  name    age   department  salary

1   haris    23          hr      25000
2   vipin    23          qa      25000
3   jithn    23          it      25000
4   rahul    23          hr      25000

```

```
http_request for adding employee

url: localhost:8000/employee/
method:POST
body:{
    "name":"vysak",
    "age":24,
    "department":"hr",
    "salary":45000
}



```
---
```
http_request for listing employee

url:localhost:8000/employee/
method:GET

```

---
```
http_request for fetching specific employee detail

url : localhost:8000/employee/4/
method:GET

```

```
http_request for updating an employee 

url:localhost:8000/employee/4/
method:PUT
body:{
    "name":"Rahul",
    "age":24,
    "department":"hr",
    "salary":30000
}

```

```
http_request for deleting  specific employee 

url:localhost:8000/employee/4/
method:DELETE
```

### Movie task

```
Movie

id      title      year     language        run_time


1          kgf1      2008      kannada           160
2          kgf2      2020      kannada           165
3          kgf3      2026      kannada           167
4          kgf4      2028      kannada           168
5          kgf5      2030      kannada           169
```

`http_request for adding new movie`

```
url: localhost:9000/movies/
method:POST
body:{
    "title":"BKU"
    "year":2026
    "language":"malayalam"
    "run_time":172
}
```
`http_request for list all movie`

```
url: localhost:9000/movies/
method:GET
```
`http_request for fetching movie detail`

```
url: localhost:9000/movies/2
method:GEt
```
`http_request for update movie`

```
url: localhost:9000/movies/2
method:PUT
body:{
    "title":"king"
    "year":2020
    "language":"hindi"
    "run_time":165
}
```
`http_request for delete movie`

```
url: localhost:9000/movies/5
method:DELEtE
```


### hospital task

```
Patient

id      name      age     token_number        status


1        ajna      40      5                    waiting
2        moosa     20      8                    waiting
3        sooraj    21      1                    completed
4        sourav    50      4                    in progress
5        ajay      22      9                    waiting
```

`http_request for adding a new patient`

```
url: localhost:7000/patient/
method:POST
body:{
    "name":"anjali"
    "age":30
    "token_number":"7"
    "status":waiting
}
```
`http_request for list all patients`

```
url: localhost:7000/patient/
method:GET
```
`http_request for fetching patient detail`

```
url: localhost:7000/patient/2
method:GET
```
`http_request for update patient detail`

```
url: localhost:7000/patient/2
method:PUT
body:{
    "name":"moosa"
    "age":25
    "token_number":2
    "status":"completed"
}
```
`http_request for delete patient`

```
url: localhost:7000/patient/2
method:DELETE
```