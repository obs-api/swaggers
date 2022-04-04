# Request to Update of BPVN Site

The objective of this request is to request the update of a BVPN site based on the Template 0003.

Please contact your Orange Representative to verify if you can use this type of request.


The request is compatible with Standard and customized catalogs.

### TYPE = U_BVPN_CUSTOM003_1

<br>
<br>

###  Structure of the `properties` section

<br>

| id         | Type     | Required  | Description|
|--------------|:-----------:|:-----------:|------------|
| `servicePoint.id`| `string`     | (1) |  Orange Single Identifier of the Service Point. This information can be found in the API Core Information in the resource _servicePoints_..       |
| `servicePoint.customerReference`      |  `string`  | (1) | Customer Reference of the Service Point.       |
| `servicePoint.reference`      |  `string`  | (1) |  Commercial Reference of the Service Point.       |
| `profile`| `string`     | required | Name of the Profile.<br>Possible values: _FDJ CONNECT OPTIMA 8M_, _FDJ CONNECT OPTIMA 18M_, _FDJ CONNECT FTTH_,   _FDJ CONNECT ULTIME_, _FDJ CONNECT CELL_   |
| `options.bandwidth`      |  `string`  | optional | *Débit*<br>Possible values: '8M', '1M', 'EXTENDED' . Only valid for the profile 'FDJ CONNECT OPTIMA 8M'      |
| `options.isAdditionalWifiNeeded`      |  `boolean`  | required |      default : 'false'   |
| `options.isMulticastNeeded`      |  `boolean`  | optional | *Multicast*    |
| `options.isQuickstartNeeded`      |  `boolean`  | optional |*Quickstart*       |
| `options.isEthernetPortNeeded`      |  `boolean`  | optional |*Ethernet complémentaire*    Boolean? |
| `options.isAnInternalAntennaNeeded`      |  `boolean`  | optional |*Antenne mobile intérieure*, only available for the profile 'FDJ CONNECT CELL'     |
| `options.isExternalAntennaNeeded`      |  `boolean`  | optional |*Antenne mobile extérieure*, only available for the profile 'FDJ CONNECT CELL'    |

<br>

(1) One of these attributes must be specified `servicePoint.id`, `servicePoint.reference`, `servicePoint.customerReference`. The API can accept the request only one Service/Product per request. By using `servicePoint.customerReference`, several Services/Products can match the value, in this case an error will be returned. 

Note: If an attribute is specified and not compatible with the selected profile, it will be ignored.

<br>

 
###  Constraints

You can use the servicePoint.customerReference, only if it is assigned to one service. 


###  Errors

The HTTP status code is 422 for all these errors

| code         | message     | Description |
|--------------|:-----------:|------------|
| 3611| RequestedAt not Valid    | The requestedAt date must be 20 days minimum and must be a working day in France.  |
| 3620| Properties item is not valid   | The 'properties' attribute is not valid due to the following error : %MSG%  |
| 3621 | Several Products match criterias    | Several Service Points mach the criteria. Disconnection can be requested on only one Service Point.   |
| 3622 | No Service Point match criteria  | No Service Point was found with the current criteria.    |
| 3623 | Internal Ordering System not available  |The ordering system is not available at the moment. The request was not accepted.   |
 