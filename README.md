# Sane-Web-API
Sane Web API - Scanner Access Now Easy
Disclaimer: work in progress - not finish or tested

## What is this API?
With this API you can access your (sane) scanners via http requests.

## How to use it

### API Documentation
#### Overview
```
/api/v0.1/scan/devices
/api/v0.1/scan/start
/api/v0.1/scan/status
/api/v0.1/scan/cancel  ~~ not implemented yet
/api/v0.1/scan/save    ~~ not implemented yet

/api/v0.1/db/reset
```

#### /api/v0.1/scan/devices
```
Type: Post
Arguments: apiKey
Return: DeviceName, Manufacturer, Model, Description, scanInitiationURL
 - Return Example: 
      {
          "0": {"device": ["test:0", "Noname", "frontend-tester", "virtual device", "http://127.0.0.1:5000/scan/startScan?scanner='test:0'", "reserved"]}, 
          "1": {"device": ["test:1", "Noname", "frontend-tester", "virtual device", "http://127.0.0.1:5000/scan/startScan?scanner='test:1'", "reserved"]}, 
      }
   Explanation: Number: {"device": [DeviceName, Manufacturer, Model, Description, scanInitiationURL, reserved]}

```

#### /api/v0.1/scan/start
```
Type: Post
Arguments: apiKey, DeviceName
Return: 
 - Return Example:
   Explanation: 
```

#### /api/v0.1/scan/status
```
Type: Post
Arguments: apiKey, scanUUID
Return: 
 - Return Example: 
   Explanation:
```

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
py -m pip install gevent
py -m pip install flask
py -m pip install flask_restful
py -m pip install numpy

install https://github.com/python-pillow/Sane

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

not determined yet (just ask if you want to use it)

## Acknowledgments

