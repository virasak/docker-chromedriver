# Docker container for creating a ChromeDriver server + webdriver-dispatcher

Includes

* ChromeDriver (Latest)
* Google Chrome (Latest Stable)
* webdriver-dispatcher (https://www.npmjs.com/package/webdriver-dispatcher)

## Create Docker service
```
docker service create --name docker-chromedriver --replicas 4 -p 5555:5555 virasak/docker-chromedriver
````

Remote WebDriver url will be:
```
http://{docker-engine}:555/webdriver
```
