
## API : System ping
### คำอธิบาย
Check all internal database connection			

### URL : /v1/system/ping				
### METHOD: GET

#### Request
##### Header
```json
{
    "accept": "application/json"
}
```

#### Response
##### Header
```json
{
    "content-type": "application/json",
}
```

##### Body
```json
// Success (status code: 200)
{
    "message" : "success"
}
```

#### Error response
```json
// Failed (status code: )
{
    "message" : "fail"
}
```

## API: Get Detail
### คำอธิบาย


### URL: /v1/:customer_number
### METHOD: POST

#### Request
##### Header
```json
{
    "accept": "application/json"
}
```

##### Body
```json
{
    "account_number": 1234567890,
}
```

| **Name**  | **Type**     | **Description**  |
|---------|----------|--------|
| account_number | int | หมายเลขบัญชี |

#### Response
##### Header
```json
{
    "content-type": "application/json",
}
```

##### Body
```json
// Success (status code: 200)
{
    "name" : "Nareenart",
    "age" : 24
}
```

#### Error response
```json
// Failed (status code: 400)
{
    "error_code":"E123400",
    "error_message": "Can't call detail"
}
```

| **Name**  | **Type**     | **Description**  |
|---------|----------|--------|
| name | string | ชื่อ |
| age | int | อายุ |