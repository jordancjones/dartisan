# dartisan
Docker container to run Laravel's Artisan command

# Usage
Run with
`
$ docker run -d -P --name artisan -v <Your Artisan Folder>:/var/www spiralout/artisan
`
If you like to have link with your database:
write on your .env file 
`
DB_HOST=db

`
and run with
`
$ docker run -d -P --name artisan <Your DB container name>:db -v <Your Artisan Folder>:/var/www spiralout/artisan
`

