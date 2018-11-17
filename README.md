# Taking Advantage of the Data Flood
> Created with Massively theme from HTML5 UP

# Creating Password Encrypted Page

1. Create the markdown page
2. Load it in browser online from GitHub Pages
3. Right click, view source, and copy
4. Goto https://robinmoisson.github.io/staticrypt/
5. Enter a password for page
6. Paste in HTML code
7. Click generate
8. Click download
9. Rename to index.html
10. Paste file into desired folder. Ex. /blog
11. Access encrypted page through folder

# Uploading Site to Amazon Web Services S3

1. Configure travis.yml through https://jekyllrb.com/docs/continuous-integration/travis-ci/
2. Add the following commands into travis.yml
```
install: 
    - gem install jekyll html-proofer bundler
    - gem install s3_website
script: 
    - bundle install
    - bundle exec jekyll build
after_success: s3_website push
```
3. Install s3_website https://github.com/laurilehmijoki/s3_website
```
gem install s3_website
```
4. Create s3_website.yml
5. On Travis for the current repo create environmental keys for AWS Access and Secret Key
6. Paste Access Key, Secret Key, and bucket id into s3_website.yml
7. When you push to GitHub, Travis and s3_website will push to AWS S3

# Amazon S3 and CloudFront

- S3 link is http://data-flood.s3-website-us-east-1.amazonaws.com
- CloudFront link is http://dgvi5kwtyqanc.cloudfront.net/
- CloudFront installation: https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/GettingStarted.html#GettingStartedUploadContent

# Airtable to JavaScript

- Copy Airtable Node.js code to here: https://repl.it/repls/MeanBronzeClosedsource
- Make a JSON Array from names list here: http://www.convertcsv.com/csv-to-json.htm
- Loop through array with JavaScript and output names

# Route53 Domain

- www.emergencydatascience.org

## Credits
```
Credits:

	Images:
		Unsplash (unsplash.com)

	Icons:
		Font Awesome (fortawesome.github.com/Font-Awesome)

	Other:
		jQuery (jquery.com)
		Misc. Sass functions (@HugoGiraudel)
		Skel (skel.io)
		Scrollex (github.com/ajlkn/jquery.scrollex)
```
