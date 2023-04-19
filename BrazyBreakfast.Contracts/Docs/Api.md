# Brazy Breakfast API   

- [Brazy Breakfast API](#brazy-breakfast-api)
    - [Create Breakfast](#create-breakfast)
        - [Create Breakfast Request](#create-breakfast-request)
        - [Create Breakfast Response](#create-breakfast-response)
    - [Get Breakfast](#get-breakfast)
        - [Get Breakfast Request](#get-breakfast-request)
        - [Get Breakfast Response](#get-breakfast-response)
    - [Update Breakfast](#update-breakfast)
        - [Update Breakfast Request](#update-breakfast-request)
        - [Update Breakfast Response](#update-breakfast-response)
    - [Delete Breakfast](#delete-breakfast)
        - [Delete Breakfast Request](#delete-breakfast-request)
        - [Delete Breakfast Response](#delete-breakfast-response)
    
## Create Breakfast

### Create Breakfast Request

```js
POST /breakfasts
```

```json
{
    "name": "Classic Homestyle Breakfast",
    "description": "Everything you need to get your day started right",
    "startDateTime": "2023-04-18T08:00:00",
    "endDateTime": "2023-04-18T11:00:00",
    "savory": [
        "Bacon",
        "Eggs",
        "Homefries",
        "Hashbrowns",
        "Biscuits",
        "Gravy"
    ],
    "sweet": [
        "Pancakes",
        "Muffins"
    ]
}
```
## Get Breakfast

### Get Breakfast Request

```js
GET /breakfasts/{{id}}
```

### Get Breakfast Response

```js
200 Ok
```

```json
{
    "id": "00000000-0000-0000-0000-000000000000",
    "name": "Classic Homestyle Breakfast",
    "description": "Everything you need to get your day started right",
    "startDateTime": "2023-04-18T08:00:00",
    "endDateTime": "2023-04-18T11:00:00",
     "lastModifiedDateTime": "2023-04-17T12:00:00",
    "savory": [
        "Bacon",
        "Eggs",
        "Homefries",
        "Hashbrowns",
        "Biscuits",
        "Gravy"
    ],
    "sweet": [
        "Pancakes",
        "Muffins"
    ]
}
```
## Update Breakfast

### Update Breakfast Request

```js
PUT /breakfasts/{{id}}
```

```json
{
    "name": "Classic Homestyle Breakfast",
    "description": "Everything you need to get your day started right",
    "startDateTime": "2023-04-18T08:00:00",
    "endDateTime": "2023-04-18T11:00:00",
    "savory": [
        "Bacon",
        "Eggs",
        "Homefries",
        "Hashbrowns",
        "Biscuits",
        "Gravy"
    ],
    "sweet": [
        "Pancakes",
        "Muffins"
    ]
}
```
### Update Breakfast Response

```js
204 No Content
```

or

```js
201 Created
```

```yml
Location: {{host}}/Breakfasts/{{id}}
```

## Delete Breakfast

### Delete Breakfast Request

```js
DELETE /breakfasts/{{id}}
```

### Delete Breakfast Response

```js
204 No Content
```
