# NodeJS in AWS course
**ATTENTION - I use Yarn as package manager**

## Task 2 (Serve SPA in AWS)
### EVALUATION CRITERIA:

- **0** - Nothing has been done. 
_(Link to repository is not provided. Nothing to check.)_
- **3** - S3 bucket has been created and configured properly. The app has been uploaded to the bucket and is available though the Internet. Nothing else has been done.
_(Link to S3 bucket/website is provided. There is no Pull Request in the YOUR OWN frontend repository.)_
- **4** - In addition to the previous work a CloudFront distribution is created and configured properly and the site is served now with CloudFront and is available through the Internet over CloudFront URL, not S3-website link (due to changes in bucket’s policy...). 
_(Link to CloudFront website is provided. S3-website shows 403 Access Denied error. There is no Pull Request in the YOUR OWN frontend repository.)_
- **5** - Serverless-finch and serverless-single-page-app plugins are added and configured. The app can be built and deployed by running npm script command. 
_(Link to CloudFront website is provided. PR with all changes is submitted in the YOUR OWN frontend repository and its link is provided for review.)_

### Results
- deployment with serverless-finch plugin on S3 (403) - http://rs-school-fe-app.s3-website-eu-west-1.amazonaws.com/
- deployment with serverless-finch plugin on CloudFront - https://d2cv8v4pgz0fxx.cloudfront.net/
- deploymenr with serverless-single-page-app-plugin on S3 (Automated to other Bucket) - http://rs-school-fe-app-cloudfront.s3-website-us-east-1.amazonaws.com/
- deploymenr with serverless-single-page-app-plugin on CloudFront (Automated to other Bucket) - https://d3owzjummp95ap.cloudfront.net/
- for deployment with serverless-finch use command `deploy`
- for deployment with serverless-single-page-app-plugin use command `cloudfront:update:build:deploy`
