# marketplace-service
## Getting Started  
#### Marketplace Service  
Marketplace Service is the platform to regulate and manage all the AI services present in our platform.
### Development
These instructions are intended to facilitate the development and testing of Marketplace Service.

### Prerequisites

* [python 3.6.5+](https://www.python.org/downloads/)
* pip 9.0.1+
* Additionally you should install the following dependency package present in requirement.txt.

### Installation
If you use Ubuntu (or any Linux distribution with APT package support) you should do the following:

#### Clone the git repository
```bash
$ git clone git@github.com:prashantramangupta/marketplace-service.git
$ cd marketplace-service
```

#### Install marketplace-service dependency using pip
```bash
$ pip install -r requirements.txt
```
#### Environment variables
Provide following environment variable in repository.py
|environment variable name|default value|
|---|---|
DB_HOST|127.0.0.1|
DB_USER|root|
DB_PASSWORD|****|
DB_NAME|default|
DB_PORT|3306|
#### Build marketplace-service (on Linux amd64 platform)
```bash
$ ./build.sh
/* This will create marketplace.zip which will be used for deployment. */
```

#### Deployment
We use AWS Lambda(serverless architecture) for deployment.
