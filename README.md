# mysql To mongo By mongify

## Getting Started

Mongify is a data translator system for moving your SQL data to MongoDB.
Mongify helps you move your data without worrying about the IDs or foreign IDs. It allows you to embed data into documents, including polymorphic associations. All this and more with just a few simple steps.

### Install gem 

`Open a terminal and type the following command:`
`$ sudo apt-get install rubygems build-essential`

OR

`$ sudo apt-get install rubygems`

OR

`$ sudo apt-get install ruby1.8-dev rubygems1.8`


#### Now install Mongify, in terminal, run:

`gem install mongify`

```
You might have to install active record database gems (you'll know if you get an error message while running mongify command)
```
#### create DataBase Config File (database.config)

````
sql_connection do
  adapter     "mysql"
  host        "localhost"
  username    "root"
  password    "passw0rd"
  database    "my_database"
  encoding  "utf8"        
# This is defaulted to 10000 but in case you want to make that smaller (on lower RAM machines)
end
````
````
mongodb_connection do
  host        "localhost"
  database    "my_database"
end
`````
