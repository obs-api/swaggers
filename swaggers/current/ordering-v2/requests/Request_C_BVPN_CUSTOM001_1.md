# Request to Creation of BPVN Site

The objective of this request is to request the deployment of a new BVPN site based on the template 001.


Please contact your Orange Representative to verify if you can use this type of request.



### TYPE = C_BVPN_CUSTOM001_1

<br>
<br>
###  Structure of the `properties` section
<br>


| id         | Type     | Description |
|--------------|:-----------:|------------|
| `network.id`      |  `string`  |Orange Single identifier of the Network where the new BVPN site must be assigned.    |
| `network.name`      |  `string`  | Name of the Network where the new BVPN site must be assigned.    |
| `billingAccount.id`      |  `string`  | Billing Account Number for invoicing the service.   |
| `billingAccount.code`      |  `string`  | Sub Billing Account Number for invoicing the service.    |
| `profile`| `string`     | Name of the Profile.   |
 
###  Constraints

You can use the servicePoint.customerReference, only if it is assigned to one service. 


###  Errors

The HTTP status code is 422 for all these errors

| code         | message     | Description |
|--------------|:-----------:|------------|
| -| -    | ----  |
| -| -    | ----  |
| -| -    | ----  |