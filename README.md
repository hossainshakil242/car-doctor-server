﻿# car-doctor-client
# car-doctor-server


## Deployment with Vercel

To deploy this project run
 create a file in root: vercel.json and put this code :

```bash
  {
  "version": 2,
  "builds": [
    {
      "src": "index.js",
      "use": "@vercel/node"
    }
  ],
  "routes": [
    {
      "src": "/(.*)",
      "dest": "/",
      "methods": [
        "GET",
        "POST",
        "PATCH",
        "DELETE",
        "OPTIONS"
      ]
    }
  ]
}
```

production: vercel --prod


and go to vercel > setting > enviroment variable > 
submit your secrate key and variable.
