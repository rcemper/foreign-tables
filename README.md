# Foreign Tables Demo
The package demonstrates a practical case of the rather new feature (2023)    
I borrowed the file Countries.csv from [CSVGEN](https://openexchange.intersystems.com/package/csvgen) for my demo   
Instead of linking the whole table just a few columns were selected.   
This is the obvious advantage of the approach:
* Collect what you need    
+ Avoid pollution of your environment with useless content   
More details on building this example in my [Article on DC](https://community.intersystems.com/post/foreign-tables-csv-action)

### Prerequisites
Make sure you have [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) and [Docker desktop](https://www.docker.com/products/docker-desktop) installed.
### Installation
Clone/git pull the repo into any local directory   https://github.com/rcemper/foreign-tables
```
$ git clone https://github.com/rcemper/foreign-tables.git
```
To build and start the container run:
```
$ docker compose up -d && docker compose logs -f
```
To open IRIS Terminal do:
```
$ docker-compose exec iris iris session iris
USER>
```
or using **WebTerminal**
```
http://localhost:42773/terminal/
```
To access IRIS System Management Portal
```
http://localhost:42773/csp/sys/UtilHome.csp
```
### How to use it
From Terminal in namespace USER just start
```
do ^DemoF
``` 
  
