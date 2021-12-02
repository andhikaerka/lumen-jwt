# Lumen JWT

Here's how to use lumen JWT

make .env file, you can copy from .env.example

## Generate API Secret

```bash
$ php artisan jwt:secret
```

## Migrate Database

```bash
php artisan migrate
```

## Run the App

```bash
$ php -S localhost:8000 -t public
```

## REGISTER

Open Postman 
```bash
(POST) 
localhost:8000/api/register
```

Fill name, email, password, password_confirmation in Body

Result

```bash
{
    "user": {
        "name": "andhika ragil",
        "email": "andhika@gmail.com",
        "updated_at": "2021-12-02T05:22:00.000000Z",
        "created_at": "2021-12-02T05:22:00.000000Z",
        "id": 2
    },
    "message": "User registered"
}
```

## LOGIN

```bash
(POST)
localhost:8000/api/login
```

Fill email and password

Result

```bash
{
    "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJodHRwOlwvXC9sb2NhbGhvc3Q6OTAwMFwvYXBpXC9sb2dpbiIsImlhdCI6MTYzODQyMjUyNywiZXhwIjoxNjM4NDI2MTI3LCJuYmYiOjE2Mzg0MjI1MjcsImp0aSI6ImUxbXdmbDVJRWozWmFzbkoiLCJzdWIiOjIsInBydiI6IjIzYmQ1Yzg5NDlmNjAwYWRiMzllNzAxYzQwMDg3MmRiN2E1OTc2ZjcifQ.sv5rUoEuVcfdyGzMms38fP3j-XvfuS_i0WUT-5Tw0F0",
    "token_type": "bearer",
    "expires_in": 3600
}
```

Thank you
