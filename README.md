# cloud-developer

## Full Stack Apps(image-filter-project)

### How to run in the localhost

#### install npm packages
```
$ npm install
```

#### run server in the localhost
```
$ npm run dev
```

#### example

```
http://localhost:8082/filteredimage?image_url=https://media.istockphoto.com/photos/kitten-with-his-paw-up-picture-id149052633
```

### How to test server in Elastic Beanstalk

example

```
http://image-filter-dev.us-east-1.elasticbeanstalk.com/filteredimage?image_url=https://media.istockphoto.com/photos/kitten-with-his-paw-up-picture-id149052633
```

### known issues
- some image files thrown error such as 
"Could not find MIME for Buffer <null>". It looks like the error related to the "jimp" library.

- "504 Gateway Time-out" error thrown if image file processing takes longer than the time limit of a load balancer.