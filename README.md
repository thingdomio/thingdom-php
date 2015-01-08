Thingdom PHP Library
===========

PHP library for v1.1 of the [Thingdom.io API](https://thingdom.io/).

## What is Thingdom?

[Thingdom](https://thingdom.io) allows you to mobile-enable your product in four lines of code with no need to develop the iOS and Android apps or create scalable cloud infrastructure. [Get Started Now!](https://thingdom.io/sign-up)

<p align="center">

<img src="https://thingdom.io/images/profile/5.png?raw=true" height="400px" />

<img src="https://thingdom.io/images/profile/2.png?raw=true" height="400px" />

</p>

## Requirements
You must have cURL for PHP installed in order to use this library.

CentOS:
```
sudo yum install php5-curl
```

Ubuntu:
```
sudo apt-get install php5-curl
```

## Getting started

First things first, [Get your free API access](https://thingdom.io/sign-up), download this library and then try the following code.

```
<?php

require_once('Thingdom.php');

// instantiate Thingdom object and authenticate
$thingdom = new Thingdom('YOUR_API_SECRET');

// look-up Thing and get back object
$thing = $thingdom->getThing('YOUR_THING_NAME');

// send a feed message
$thing->feed('FEED_CATEGORY', 'MESSAGE');

// send a status update
$thing->status('KEY', 'VALUE');

```

## Ideas for Library Usage

1. Programmatically trigger push notifications, feed messages, and real-time status updates from your PHP code.
2. Remotely monitor any interaction with your PHP application or web server.
3. With our quick drop-in integration and simple API calls you can mobile-enable your PHP application in a matter of hours, even customizing the mobile experience for your end-users. 
