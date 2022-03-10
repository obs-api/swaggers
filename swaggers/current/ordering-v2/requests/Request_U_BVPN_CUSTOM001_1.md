

# Request to Update of BPVN Site

The objective of this request is to request the disconnection of a BVPN site.

The request is compatible with Standard and customized catalogs.

### TYPE = U_BVPN_CUSTOM001_1

<br>
<br>
###  Structure of the `properties` section
<br>


| id         | Type     | Description |
|--------------|:-----------:|------------|
| `servicePoint.id`| `string`     | Orange Single Identifier of the Service Point. This information can be found in the API Core Information in the resource _servicePoints_..       |
| `servicePoint.customerReference`      |  `string`  | Customer Reference of the Service Point.       |
| `servicePoint.reference`      |  `string`  | Commercial Reference of the Service Point.       |
| `location.name`      |  `string`  |  Name of the location where the service must be installed. |
| `location.localCompany`      |  `string`  | Name of the Local Company  |
| `location.localCompanyNumber`      |  `string`  | Number of the Local Company corresponding to the SIREN.  |
| `location.address.street`      |  `string`  | Main street information. |
| `location.address.extendedStreet`      |  `string`  | Complementary information allowing to facilitate the elligibily of the Offer.  |
| `location.address.postalCode`      |  `string`  | Postal Code of the Location. For France, must be a 5 digits number.  |
| `location.address.city`      |  `string`  | Name of the City  |
| `contacts.primary.title`      |  `string`  |  Title of the person. Authorized Values are: M., Mrs.  |
| `contacts.primary.firstName`      |  `string`  | First name of the person.   |
| `contacts.primary.lastName`      |  `string`  |  Last name of the person  |
| `contacts.primary.phone`      |  `string`  |   Phone Number of the person. The format must be + (TODO) |
| `contacts.primary.mobile`      |  `string`  |   Mobile Phone Number of the person. The format must be + (TODO) |
| `contacts.primary.email`      |  `string`  |  Email of the person. |
| `contacts.secondary.title`      |  `string`  | Title of the person. Authorized Values are: M., Mrs.    |
| `contacts.secondary.firstName`      |  `string`  |  First name of the person.   |
| `contacts.secondary.lastName`      |  `string`  |Last name of the person   |
| `contacts.secondary.phone`      |  `string`  | Phone Number of the person. The format must be + (TODO)   |
| `contacts.secondary.mobile`      |  `string`  |   Mobile  Phone Number of the person. The format must be + (TODO) |
| `contacts.secondary.email`      |  `string`  |  Email of the person.    |
 
###  Constraints

You can use the servicePoint.customerReference, only if it is assigned to one service. 


###  Errors

The HTTP status code is 422 for all these errors

| code         | message     | Description |
|--------------|:-----------:|------------|
| -| -    | ----  |
| -| -    | ----  |
| -| -    | ----  |