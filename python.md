# Python Links

## Pipenv

- https://docs.pipenv.org/advanced/#configuration-with-environment-variables - fix it when its bugging
- install specific packages
```
$ pipenv install --deploy
```
- location of where to active
```
pipenv --where
```
- location of venv
```
pipenv --venv
```


## OOP / Classes

- https://favtutor.com/blogs/import-class-from-another-file-python - Importing files

## Scripting

- https://www.danielherediamejias.com/scraping-on-instagram-with-instagram-scraper-and-python/
- https://www.jcchouinard.com/python-for-seo/
- https://brightdata.com/blog/how-tos/how-to-scrape-social-media-guide

## Sympy

- https://scipy-lectures.org/packages/sympy.html
- https://docs.sympy.org/latest/explanation/gotchas.html#gotchas
    - Beware
- https://docs.sympy.org/latest/tutorials/intro-tutorial/basic_operations.html
- https://docs.sympy.org/latest/modules/functions/index.html#functions-contents
- https://docs.sympy.org/latest/tutorials/intro-tutorial/calculus.html

## Jupyter Notebooks

- https://ploomber.io/blog/clean-nbs/ (great article)
- https://notebook.community/
- https://towardsdatascience.com/write-markdown-latex-in-the-jupyter-notebook-10985edb91fd - Markdown
- https://www.markdownguide.org/basic-syntax/ - more markdown
- https://www.tablesgenerator.com/markdown_tables - Generate markdown tables
- https://towardsdatascience.com/jupyter-best-practices-that-will-save-you-a-lot-of-headaches-67e1df45e24d
- https://stackoverflow.com/questions/34734714/ipython-jupyter-uploading-folder - Import an entire zip
- https://www.dataquest.io/blog/jupyter-notebook-tips-tricks-shortcuts/

## Matplotlib

### Interactive plots in vscode
- https://www.mssqltips.com/sqlservertip/7607/python-matplotlib-interactive-data/

## Pandas

### Writing to excel
- https://pythonbasics.org/write-excel/

### Compare two dataframes / series
- https://pandas.pydata.org/docs/reference/api/pandas.Series.equals.html

### Compare two datasets
- https://pandas.pydata.org/docs/reference/api/pandas.Series.compare.html

### Apply function to every row
- https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.apply.html

### Add new column with values based on other columns
- https://www.dataquest.io/blog/tutorial-add-column-pandas-dataframe-based-on-if-else-condition/

### Pandas group by
- https://www.geeksforgeeks.org/how-to-count-unique-values-in-a-pandas-groupby-object/

### Latex
- https://pandas.pydata.org/pandas-docs/version/0.21/generated/pandas.DataFrame.to_latex.html

### Read in SQL
- https://blog.panoply.io/how-to-read-a-sql-query-into-a-pandas-dataframe - Can read your sql into a temporary csv and then read it into a pandas dataframe to improve speed


## Geopandas

### geo-series
- https://geopandas.org/en/stable/docs/reference/geoseries.html

### Projections
- https://spatialreference.org/

### Color maps
- https://matplotlib.org/stable/tutorials/colors/colormaps.html
- https://matplotlib.org/mpl-third-party/#colormaps-and-styles

### Markersize
- https://gis.stackexchange.com/questions/241612/change-marker-size-in-plot-with-geopandas

### Labelling polygons
- https://github.com/shotleft/how-to-python/blob/master/How%20it%20works%20-%20labelling%20districts%20in%20GeoPandas.ipynb

### Spatial Joins
- https://www.practicaldatascience.org/html/gis_spatial_joins.html

### Overlaps
- https://geobgu.xyz/py/geopandas2.html#geopandas-geometric-relations

### Geometric files
- https://gisgeography.com/arcgis-shapefile-files-types-extensions/
- https://spatialreference.org/ref/epsg/ - EPSG codes
- https://gisgeography.com/arcgis-shapefile-files-types-extensions/
- https://www.youtube.com/watch?v=BopzJ4rXoPA
- http://geokov.com/education/latitude-longitude.aspx - Basics on lat longs

### Map Styling
- https://www.youtube.com/watch?v=ff3At9NRcsg&list=PLewNEVDy7gq3DjrPDxGFLbHE4G2QWe8Qh&index=10
- https://www.google.com/search? - map inspiration


## Django

- https://www.appsloveworld.com/django/100/91/how-to-set-timeout-for-django-rest-http-request - Set timeout

### Latency

- https://www.dabapps.com/blog/api-performance-profiling-django-rest-framework/
- https://restfulapi.net/caching/

### Memory Usage
- https://pythonspeed.com/articles/measuring-memory-python/

### Timing python functions

- https://www.geeksforgeeks.org/time-process_time-function-in-python/
- https://www.geeksforgeeks.org/time-perf_counter-function-in-python/

### Get users IP Address
- https://stackoverflow.com/questions/4581789/how-do-i-get-user-ip-address-in-django


### Passwords
- https://blog.mozilla.org/webdev/2012/06/08/lets-talk-about-password-storage/ - The good strategy
- https://wiki.mozilla.org/WebAppSec/Secure_Coding_Guidelines#Password_Storage - Nice strategies for migrating hashes
- http://fredericiana.com/2010/10/12/adding-support-for-stronger-password-hashes-to-django/ - django hashing
- https://developer.okta.com/blog/2021/03/05/ultimate-guide-to-password-hashing-in-okta - great article
- https://crypto.stackexchange.com/questions/46550/benchmark-differences-between-sha-512-and-bcrypt/46552#46552 - bcrypt

### Logging
- https://12factor.net/logs - 12 Factor App

### Decorators
- https://www.saltycrane.com/blog/2009/11/trying-out-retry-decorator-python/
- https://www.saltycrane.com/blog/2010/04/using-python-timeout-decorator-uploading-s3/

### Deploying
- Set allowed host in settings
- Set static folder
- Ensure you are starting server on 0.0.0.0 and allowing traffic over given port
#### GUnicorn
- https://www.digitalocean.com/community/tutorials/how-to-set-up-django-with-postgres-nginx-and-gunicorn-on-ubuntu-20-04
- Directory to find Gunicorn
```
etc/systemd/system
```

### Docker
- https://mherman.org/presentations/dockercon-2018/#1
- https://testdriven.io/blog/dockerizing-django-with-postgres-gunicorn-and-nginx/

### Systemd
- https://ubuviz.com/blog/2021/06/09/deploying-django-based-app-systemd/
- https://www.shellhacks.com/journalctl-tail-service-logs-systemd-journal/
```
journalctl -u nginx.service -n 100 --no-pager
```

### Set dynamic hosts IP Address
- https://stackoverflow.com/questions/47277541/how-to-dynamically-add-ec2-ip-addresses-to-django-allowed-hosts


## Dash

- https://dash-bootstrap-components.opensource.faculty.ai/
- https://dash.plotly.com/dash-core-components
- https://medium.com/plotly/dash-is-react-for-python-r-and-julia-c75822d1cc24

### Deploy with Elastic Beanstalk
- https://www.youtube.com/watch?v=hhVuUESnl6Q

### Plotly
- https://www.geeksforgeeks.org/python-plotly-tutorial/

## Databases

### MySQL Client
- https://stackoverflow.com/questions/50604948/python3-pipenv-install-mysqlclient

### Errors
- https://dev.mysql.com/doc/connector-python/en/connector-python-api-errors.html
- https://stackoverflow.com/questions/11293380/django-catching-integrity-error-and-showing-a-customized-message-using-template/11293459#11293459

## AWS

### SNS SQS
- https://perandrestromhaug.com/posts/writing-an-sqs-consumer-in-python/
- https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html

### ELB Health Checks
- https://sanyambansal.wordpress.com/2017/06/26/how-to-make-djangos-allowed_hosts-work-with-aws-elb-health-checks/
- https://tech.octopus.energy/news/2016/05/05/django-elb-health-checks.html


## Firebase

- https://www.freecodecamp.org/news/how-to-get-started-with-firebase-using-python/

### Push Notifications
- https://github.com/firebase/firebase-admin-python/blob/fb64981f08228aae2c3742c4e507d9793c16c17e/snippets/messaging/cloud_messaging.py#L67-L84


## Webscraping

- https://www.scrapingbee.com/blog/web-scraping-with-scrapy/
- https://www.scrapingbee.com/blog/selenium-python/
- https://www.scrapingbee.com/blog/web-scraping-101-with-python/
- https://www.scrapingbee.com/blog/web-scraping-without-getting-blocked/
- https://en.wikipedia.org/wiki/List_of_HTTP_header_fields - Headers
- https://antoinevastel.com/ - Fingerprinting
- https://www.cloudflare.com/learning/ssl/transport-layer-security-tls/ - Changing TLS Fingerprint
- https://hussainaliakbar.github.io/restricting-tls-version-and-cipher-suites-in-python-requests-and-testing-with-wireshark/ - Proxies
- https://www.bestproxyreviews.com/rotating-proxies/
- https://www.charlesproxy.com/

## Testing

- https://www.360logica.com/blog/sneak-peek-test-framework-test-pyramid-testing-pyramid/
- https://www.sisense.com/blog/rest-api-testing-strategy-what-exactly-should-you-test/

- https://www.chaijs.com/
- https://www.youtube.com/watch?v=sB2HHrezQOo&t=3s - Use this for testing with postman

