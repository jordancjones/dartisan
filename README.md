# dartisan
Docker container to run Laravel's Artisan command

# Usage
Run with
```
$ docker run -P -v </Your/Absolute/Path/To/laravel/folder>:/var/www spiralout/dartisan <artisan command eg. list>
```
If you like to have link with your database:
write on your .env file 

```
DB_HOST=db
```
and run with
```
$ docker run -d -P --name artisan <Your DB container name>:db -v </Your/Absolute/Path/To/laravel/folder>:/var/www spiralout/dartisan <artisan command eg. make:auth>
```

