
### Create User
![create Users](image.png)

```
curl --location 'localhost:5001/users' \
--header 'Content-Type: application/json' \
--data-raw '{
    "email": "Atharva@example.com",
    "name": "Atharva"
}'

```

### Get User
![Get User](image-1.png)

```
curl --location 'localhost:5001/users/3'
```

### Create Order
![Create Order](image-2.png)

```
curl --location 'localhost:5002/orders' \
--header 'Content-Type: application/json' \
--data '{
    "user_id": 1,
    "product": "iPhone"
}'
```


### Get Order
![Get Order](image-3.png)

```
curl --location 'localhost:5002/orders/3'
```