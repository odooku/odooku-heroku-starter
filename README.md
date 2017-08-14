```
$ heroku create --buildpack https://github.com/odooku/odooku-buildpack.git#10.0
$ heroku addons:create heroku-postgresql:hobby-basic
$ heroku addons:create heroku-redis:hobby-dev
$ heroku config:set AWS_ACCESS_KEY_ID=<your_aws_key>
$ heroku config:set AWS_SECRET_ACCESS_KEY=<your_aws_secret>
$ heroku config:set AWS_REGION=<your_aws_region>
$ heroku config:set S3_BUCKET=<your_s3_bucket_name>
$ git push heroku master
$ heroku run odooku database preload
```