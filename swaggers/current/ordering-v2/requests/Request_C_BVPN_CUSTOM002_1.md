# Request to Creation of BPVN Site

The objective of this request is to request the deployment of a new BVPN site based on the template 002.


Please contact your Orange Representative to verify if you can use this type of request.


### TYPE = C_BVPN_CUSTOM002_1

<br>
<br>
###  Structure of the `properties` section
<br>


| id         | Type     | Description |
|--------------|:-----------:|------------|
| `servicePoint.id`| `string`     | Orange Single Identifier of the Service Point. This information can be found in the API Core Information in the resource _servicePoints_..       |
| `servicePoint.customerReference`      |  `string`  | Customer Reference of the Service Point.       |
| `servicePoint.reference`      |  `string`  | Commercial Reference of the Service Point.       |
 
###  Constraints

You can use the servicePoint.customerReference, only if it is assigned to one service. 


###  Errors

The HTTP status code is 422 for all these errors

| code         | message     | Description |
|--------------|:-----------:|------------|
| -| -    | ----  |
| -| -    | ----  |
| -| -    | ----  |