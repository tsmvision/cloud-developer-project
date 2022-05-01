# cloud-developer

## Full Stack Apps(image-filter-project)

### How to use

#### localhost

```
http://localhost:8082/filteredimage?image_url=https://media.istockphoto.com/photos/kitten-with-his-paw-up-picture-id149052633
```

#### elasticbeanstalk

```
http://image-filter-dev.us-east-1.elasticbeanstalk.com/ilteredimage?image_url=https://media.istockphoto.com/photos/kitten-with-his-paw-up-picture-id149052633
```

##### known issues
- some image file thrown error such as 
"Could not find MIME for Buffer <null>". It looks related with "jimp" library.

- "504 Gateway Time-out" error thrown if image file processing takes longer than the time limit of a load balancer.