# ![LOGO](logo.png) OpenALPR Cloud **flow**ground Connector

## Description

A generated **flow**ground connector for the OpenALPR Cloud API (version 2.0.1).

Generated from: https://api.apis.guru/v2/specs/openalpr.com/2.0.1/swagger.json<br/>
Generated at: 2019-06-06T16:12:54+03:00

## API Description

The OpenALPR Cloud API allows you to send images to the cloud for processing. 
The image will be analyzed for license plates and vehicle make/models.  The results 
are returned in JSON format


## Authorization

This API does not require authorization.

## Actions

### Get a list of available results for plate and vehicle recognition

### Send an image for OpenALPR to analyze and provide metadata back<br/>
> The image is sent as a file using a form data POST

#### Input Parameters
* `secret_key` - _required_ - The secret key used to authenticate your account.  You can view your 
secret key by visiting 
https://cloud.openalpr.com/

* `recognize_vehicle` - _optional_ - If set to 1, the vehicle will also be recognized in the image
This requires an additional credit per request

    Possible values: 0, 1.
* `country` - _required_ - Defines the training data used by OpenALPR.  "us" analyzes 
North-American style plates.  "eu" analyzes European-style plates.

This field is required if using the "plate" task

* `state` - _optional_ - Corresponds to a US state or EU country code used by OpenALPR pattern 
recognition.  For example, using "md" matches US plates against the 
Maryland plate patterns.  Using "fr" matches European plates against 
the French plate patterns.

* `return_image` - _optional_ - If set to 1, the image you uploaded will be encoded in base64 and 
sent back along with the response

    Possible values: 0, 1.
* `topn` - _optional_ - The number of results you would like to be returned for plate 
candidates and vehicle classifications

* `prewarp` - _optional_ - Prewarp configuration is used to calibrate the analyses for the 
angle of a particular camera.  More information is available here
http://doc.openalpr.com/accuracy_improvements.html#calibration


### Send an image for OpenALPR to analyze and provide metadata back<br/>
> The image is sent as base64 encoded bytes.

#### Input Parameters
* `secret_key` - _required_ - The secret key used to authenticate your account.  You can view your 
secret key by visiting 
https://cloud.openalpr.com/

* `recognize_vehicle` - _optional_ - If set to 1, the vehicle will also be recognized in the image
This requires an additional credit per request

    Possible values: 0, 1.
* `country` - _required_ - Defines the training data used by OpenALPR.  "us" analyzes 
North-American style plates.  "eu" analyzes European-style plates.

This field is required if using the "plate" task

* `state` - _optional_ - Corresponds to a US state or EU country code used by OpenALPR pattern 
recognition.  For example, using "md" matches US plates against the 
Maryland plate patterns.  Using "fr" matches European plates against 
the French plate patterns.

* `return_image` - _optional_ - If set to 1, the image you uploaded will be encoded in base64 and 
sent back along with the response

    Possible values: 0, 1.
* `topn` - _optional_ - The number of results you would like to be returned for plate 
candidates and vehicle classifications

* `prewarp` - _optional_ - Prewarp configuration is used to calibrate the analyses for the 
angle of a particular camera.  More information is available here
http://doc.openalpr.com/accuracy_improvements.html#calibration


### Send an image for OpenALPR to analyze and provide metadata back<br/>
> The image is sent as a URL.  The OpenALPR service will download the image <br/>
> and process it

#### Input Parameters
* `image_url` - _required_ - A URL to an image that you wish to analyze

* `secret_key` - _required_ - The secret key used to authenticate your account.  You can view your 
secret key by visiting 
https://cloud.openalpr.com/

* `recognize_vehicle` - _optional_ - If set to 1, the vehicle will also be recognized in the image
This requires an additional credit per request

    Possible values: 0, 1.
* `country` - _required_ - Defines the training data used by OpenALPR.  "us" analyzes 
North-American style plates.  "eu" analyzes European-style plates.

This field is required if using the "plate" task

* `state` - _optional_ - Corresponds to a US state or EU country code used by OpenALPR pattern 
recognition.  For example, using "md" matches US plates against the 
Maryland plate patterns.  Using "fr" matches European plates against 
the French plate patterns.

* `return_image` - _optional_ - If set to 1, the image you uploaded will be encoded in base64 and 
sent back along with the response

    Possible values: 0, 1.
* `topn` - _optional_ - The number of results you would like to be returned for plate 
candidates and vehicle classifications

* `prewarp` - _optional_ - Prewarp configuration is used to calibrate the analyses for the 
angle of a particular camera.  More information is available here
http://doc.openalpr.com/accuracy_improvements.html#calibration


## License

**flow**ground :- Telekom iPaaS / openalpr-com-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
