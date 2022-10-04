
# Rivoj-Yulduz Backend Api

Telegram botdan dizimnen otkenler haqqindagi
 magliwmatlardi admin koriw ushin admin panel
islew kerek.


## Admin
####  login

```http
  GET /api/login
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `phone` | `string` | **Required**.  |
| `password` | `string` | **Required**. |

#### leads

```http
  GET /api/leads
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`| `integer` | **Required**.  |
| `tg_id`| `integer` | **Required**.  |
| `name`| `string` | ****.  |
| `surname`| `string` | ****.  |
| `phone`| `string` | ****.  |
| `company`| `string` | ****.  |
| `status`| `string` | start,signed,joined  |

### bir leadga kirgende 
#### 1 userge kirgende qaysi menularga neshe marte kirgenin shigarip beriw kerek.
 

```http
  GET /api/leads/{id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`| `integer` | **Required**.  |
| `menu_id`| `integer` | **Required**.  |
| `menu_name`| `string` | ****.  |
| `count`| `integer`| *****|

### menyular 
 
```http
  GET /api/menu
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`| `integer` | **Required**.  |
| `name`| `string` | ****.  |
| `count`| `integer`| *****|


### 1 menu ga kirgende 
 
```http
  GET /api/menu/{id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`| `integer` | **Required**.  |
| `name`| `string` | ****.  |
| `count`| `integer`| *****|

### pikirler 
 
```http
  GET /api/reviews
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`| `integer` | **Required**.  |
| `review`| `string` | ****.  |
| `name`| `string`| *****|

### dizaynerlerdin reytingi  
 
```http
  GET /api/rating
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`| `integer` | **Required**.  |
| `name`| `string` | ****.  |
| `rating`| `integer`| *****|
