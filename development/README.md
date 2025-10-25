<br>

### Development Notes

**GitHub Actions**
* [Actions & Secure Deliveries](https://docs.github.com/en/actions/deployment/security-hardening-your-deployments/configuring-openid-connect-in-amazon-web-services)
* [Actions & S3](https://docs.github.com/en/actions/deployment/security-hardening-your-deployments/configuring-openid-connect-in-amazon-web-services#requesting-the-access-token)
* Connecting GitHub Actions to Amazon Web Services via [IAM (Identity & Access Management) Roles](https://aws.amazon. com/blogs/security/use-iam-roles-to-connect-github-actions-to-actions-in-aws/)

<br>

**Secure Static Site Options**
* [How do I use CloudFront to serve HTTPS requests for my Amazon S3 bucket?](https://repost.aws/knowledge-center/cloudfront-https-requests-s3)
* [How do I use CloudFront to serve a static website that’s hosted on Amazon S3?](https://repost.aws/knowledge-center/cloudfront-serve-static-website)
* [CloudFront Distributions](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/distribution-web-values-specify.html)
* [Secure](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/getting-started-secure-static-website-cloudformation-template.html)
* [Manage how long content stays in the cache (expiration)](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/Expiration.html)


<br>

**Static Sites**
* [Basic](https://docs.aws.amazon.com/AmazonS3/latest/userguide/HostingWebsiteOnS3Setup.html)

<br>

**JavaScript Libraries**
* [Google Fonts](https://developers.google.com/fonts/docs/getting_started)
* [Google Libraries for Developers](https://developers.google.com/speed/libraries)
* [CDN (Content Delivery Network) JavaScript Libraries](https://cdnjs.com)


<br>
<br>

### Server

Launch an interactive environment via

```shell
docker run --rm -i -t -p 8080:80 -w /app 
  --mount type=bind,src="$(pwd)",target=/app 
    dynamic
```

Subsequently, launch a web server via

```shell
nginx -g 'daemon off;'
```

The URL is

```text
http://localhost:8080
```

Note, for an immediate web server launch $\rightarrow$

```shell
docker run --rm -i -t -p 8080:80 -w /app 
  --mount type=bind,src="$(pwd)",target=/app 
    dynamic nginx -g 'daemon off;'
```

<br>
<br>

<br>
<br>

<br>
<br>

<br>
<br>
