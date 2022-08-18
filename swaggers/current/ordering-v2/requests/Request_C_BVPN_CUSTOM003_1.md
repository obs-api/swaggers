# Request to Creation of BPVN Site

The objective of this request is to request the deployment of a new BVPN site based on the template 003.


Please contact your Orange Representative to verify if you can use this type of request.


### TYPE = C_BVPN_CUSTOM003_1

<br>
<br>

###  Structure of the `properties` section

<br>


| id         | Type     | required | Description |
|--------------|:-----------:|:-----------:|------------|
| `network.id`      |  `string` | (1) |Orange Single identifier of the Network where the new BVPN site must be assigned.    |
| `network.name`      |  `string`  |(1) | Name of the Network where the new BVPN site must be assigned.    |
| `billingAccount.id`      |  `string`  |(2) | Billing Account Number for invoicing the service.   |
| `billingAccount.code`      |  `string`  |(2) | Sub Billing Account Number for invoicing the service.    |
| `profile`| `string`     | required | Name of the Profile.<br>Possible values: _FDJ CONNECT OPTIMA 8M_, _FDJ CONNECT OPTIMA 18M_, _FDJ CONNECT FTTH_,   _FDJ CONNECT ULTIME_, _FDJ CONNECT CELL_   |
| `location.name`      |  `string`  | required |  Name of the location where the service must be installed. The max size is 20 characters.|
| `location.localCompany`      |  `string`  | optional | Name of the Local Company  |
| `location.localCompanyLegalNumber`      |  `string`  | optional | Number of the Local Company corresponding to the SIREN.  |
| `location.building`      |  `string`  | optional | Building name. The max size is 50 characters. |
| `location.buildingCode`      |  `string`  | optional | Building Code provided by ARCEP. The max size is 50 characters. |
| `location.name`      |  `string`  | required |  Name of the location where the service must be installed. The max size is 20 characters.|
| `location.stair`      |  `string`  | optional | Stair of the location. The max size is 50 characters. |
| `location.floor`      |  `string`  | optional | Floor number. The max size is 50 characters. |
| `location.room`      |  `string`  | optional | Room number. The max size is 50 characters. |
| `location.address.street`      |  `string`  | required | Main street information. The max size is 50 characters.|
| `location.building`      |  `string`  | optional | Building name. The max size is 50 characters. |
| `location.address.postalCode`      |  `string`  | required | Postal Code of the Location. For France, must be a 5 digits number.  |
| `location.address.city`      |  `string`  | required | Name of the City. The max size is 50 characters.  |
| `contacts.primary.title`      |  `string`  | required |  Title of the person. Authorized Values are: M., Mrs.  |
| `contacts.primary.firstName`      |  `string`  | required | First name of the person.   |
| `contacts.primary.lastName`      |  `string`  | required |  Last name of the person  |
| `contacts.primary.phone`      |  `string`  | required |   Phone Number of the person. The format must be + (TODO) |
| `contacts.primary.mobile`      |  `string`  | required |   Mobile Phone Number of the person. The format must be + (TODO) |
| `contacts.primary.email`      |  `string`  | required |  Email of the person. |
| `contacts.secondary.title`      |  `string`  | optional | Title of the person. Authorized Values are: M., Mrs.    |
| `contacts.secondary.firstName`      |  `string`  | optional |  First name of the person.   |
| `contacts.secondary.lastName`      |  `string`  | optional |Last name of the person   |
| `contacts.secondary.phone`      |  `string`  | optional | Phone Number of the person. The format must be + (TODO)   |
| `contacts.secondary.mobile`      |  `string`  | optional |   Mobile  Phone Number of the person. The format must be + (TODO) |
| `contacts.secondary.email`      |  `string`  | optional | Email of the person.    |
| `options.bandwidth`      |  `string`  | optional | *Débit*<br>Possible values: '8M', '1M', 'EXTENDED' . Only valid for the profile 'FDJ CONNECT OPTIMA 8M'      |
| `options.isAdditionalWifiNeeded`      |  `boolean`  | required |      default : 'false'   |
| `options.isMulticastNeeded`      |  `boolean`  | optional | *Multicast*    |
| `options.isQuickstartNeeded`      |  `boolean`  | optional |*Quickstart*       |
| `options.isEthernetPortNeeded`      |  `boolean`  | optional |*Ethernet complémentaire*    Boolean? |
| `options.isAnInternalAntennaNeeded`      |  `boolean`  | optional |*Antenne mobile intérieure*, only available for the profile 'FDJ CONNECT CELL'     |
| `options.isExternalAntennaNeeded`      |  `boolean`  | optional |*Antenne mobile extérieure*, only available for the profile 'FDJ CONNECT CELL'    |


<br>

(1)

(2) At least one of these value must be provided

(3)

(4)


### Options required for _FDJ CONNECT OPTIMA 8M_


| id         | Type     | required | Description |
|--------------|:-----------:|:-----------:|------------|
| `options.bandwidth`      |  `string`  | optional | *Débit*<br>Possible values: '8M', '1M', 'EXTENDED' . Only valid for the profile 'FDJ CONNECT OPTIMA 8M'      |
| `options.isAdditionalWifiNeeded`      |  `boolean`  | required |      default : 'false'   |
| `options.isMulticastNeeded`      |  `boolean`  | optional | *Multicast*    |
| `options.isQuickstartNeeded`      |  `boolean`  | optional |*Quickstart*       |
| `options.isEthernetPortNeeded`      |  `boolean`  | optional |*Ethernet complémentaire*    Boolean? |



### Options required for _FDJ CONNECT OPTIMA 18M_

| id         | Type     | required | Description |
|--------------|:-----------:|:-----------:|------------|
| `options.isAdditionalWifiNeeded`      |  `boolean`  | required |      default : 'false'   |
| `options.isMulticastNeeded`      |  `boolean`  | optional | *Multicast*    |
| `options.isQuickstartNeeded`      |  `boolean`  | optional |*Quickstart*       |
| `options.isEthernetPortNeeded`      |  `boolean`  | optional |*Ethernet complémentaire*    Boolean? |


### Options required for _FDJ CONNECT FTTH_

| id         | Type     | required | Description |
|--------------|:-----------:|:-----------:|------------|
| `options.isAdditionalWifiNeeded`      |  `boolean`  | required |      default : 'false'   |
| `options.isMulticastNeeded`      |  `boolean`  | optional | *Multicast*    |
| `options.isQuickstartNeeded`      |  `boolean`  | optional |*Quickstart*       |
| `options.isEthernetPortNeeded`      |  `boolean`  | optional |*Ethernet complémentaire*    Boolean? |


### Options required for  _FDJ CONNECT ULTIME_

| id         | Type     | required | Description |
|--------------|:-----------:|:-----------:|------------|
| `options.isAdditionalWifiNeeded`      |  `boolean`  | required |      default : 'false'   |
| `options.isMulticastNeeded`      |  `boolean`  | optional | *Multicast*    |
| `options.isQuickstartNeeded`      |  `boolean`  | optional |*Quickstart*       |
| `options.isEthernetPortNeeded`      |  `boolean`  | optional |*Ethernet complémentaire*    Boolean? |
 


### Options required for   _FDJ CONNECT CELL_

| id         | Type     | required | Description |
|--------------|:-----------:|:-----------:|------------|
| `options.isAdditionalWifiNeeded`      |  `boolean`  | required |      default : 'false'   |
| `options.isMulticastNeeded`      |  `boolean`  | optional | *Multicast*    |
| `options.isQuickstartNeeded`      |  `boolean`  | optional |*Quickstart*       |
| `options.isEthernetPortNeeded`      |  `boolean`  | optional |*Ethernet complémentaire*    Boolean? |
| `options.isAnInternalAntennaNeeded`      |  `boolean`  | optional |*Antenne mobile intérieure*,    |
| `options.isExternalAntennaNeeded`      |  `boolean`  | optional |*Antenne mobile extérieure*,    |







Note: If an attribute is specified and not compatible with the selected profile, it will be ignored.


## MAPPING RULES - Temporary (need to move in the Internal documentation)



| id         | Type     | required | Description |
|--------------|:-----------:|:-----------:|------------|
| `options.bandwidth`      |  `string`  | optional |  the default is '8M' and the value code is sent for the selected bandwidth     |
| `options.isAdditionalWifiNeeded`      |  `boolean`  | optional |  if (value=false) send WIFI0002 with quantify=1 , if true  WIFI0002 with quantify=2    |
| `options.isMulticastNeeded`      |  `boolean`  |  if (value=false) nothing is sent , if true  the option code is sent for the optionn MULTICAS01  |     |
| `options.isQuickstartNeeded`      |  `boolean`  |  if (value=false) nothing is sent , if true  the option code is sent for the optionn QUICKSMALL or QUICKCORPO following the selected profile |      |
| `options.isEthernetPortNeeded`      |  `boolean`  | if (value=false) nothing is sent , if true  the option code is sent for the optionn WIFI0004   |  |
| `options.isAnInternalAntennaNeeded`      |  `boolean`  | if (value=false) nothing is sent , if true  the option code is sent for the optionn ANTENNEINT  |    |
| `options.isExternalAntennaNeeded`      |  `boolean`  | if (value=false) nothing is sent , if true  the option code is sent for the optionn ANTENNEEXT  |    |



<br>
<br>
<br>


###  Constraints

You can use the servicePoint.customerReference, only if it is assigned to one service. 


###  Business Errors

The HTTP status code is 422 for all these errors

| code         | message     | Description |
|--------------|:-----------:|------------|
| 3623 | Internal Ordering System not available  |The ordering system is not available at the moment. The request was not accepted.   |
| 3630 | Not authorized  |You are not authorized to send request on this Network.   |
| 3631 | Several Networks  | Not possible to determine a single network based on the criteria provided. |
 