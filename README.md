# get started
clone a json-server from: ```git clone https://github.com/typicode/json-server.git```

Run ``` json-server --watch db.json``` to start the mock server using the default data file

By default the server runs on port 3000 so the URL will be: http://localhost:3000/posts

A differnt oport can be specified by: ```json-server --watch db.json --port 3004```

Run ``` touch mydata.json``` inside the root of ```json-server``` to create your own data file

Customise routes to simulate your own API, example:
``` 
#routes.json
{
  "/api/*": "/$1"
}

```
will support accessing posts via: http://localhost:3000/api/posts
