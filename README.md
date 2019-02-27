# Sane-Web-API-python-
Sane Web API - Scanner Access Now Easy

## What is this API?
With this API you can access your (sane) scanners via http requests.

## How to use it

### API Documentation
POST:
```
/api/v0.1/scan/devices
/api/v0.1/scan/start
/api/v0.1/scan/status
/api/v0.1/scan/cancel

/api/v0.1/db/reset
```

#### /api/v0.1/scan/devices
'''
Type: Post
Arguments: apiKey
Return Json: devices
 - Return Example: 
       {
          "0": {"device": ["test:0", "Noname", "frontend-tester", "virtual device", "http://127.0.0.1:5000/scan/startScan?scanner='test:0'", "http://127.0.0.1:5000/scan/startScan?scanner='test:0'"]}, 
          "1": {"device": ["test:1", "Noname", "frontend-tester", "virtual device", "http://127.0.0.1:5000/scan/startScan?scanner='test:1'", "http://127.0.0.1:5000/scan/startScan?scanner='test:1'"]}, 
      }
'''


## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

What things you need to install the software and how to install them

Linux (tested with Ubuntu 18.04 Server) <br />
[Sane](https://www.sane-project.org//) <br />
Python3 <br />

```
Give examples
```

### Installing

A step by step series of examples that tell you how to get a development env running

Say what the step will be

```
Give the example
```

And repeat

```
until finished
```

End with an example of getting some data out of the system or using it for a little demo

## Deployment

Add additional notes about how to deploy this on a live system

## Built With



## Authors

* **Axel Hieber** - *Initial work* - [Axel Hieber](https://github.com/axelhieber)


## License

not determined yet (ask if you want to use it)

## Acknowledgments

