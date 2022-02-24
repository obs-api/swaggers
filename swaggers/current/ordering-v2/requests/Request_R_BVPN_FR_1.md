

# Request to Disconnect of BPVN Site

The objective of this request is to request the disconnection of a BVPN site.

The request is compatible with Standard and customized catalogs.

### TYPE = R_BVPN_1

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