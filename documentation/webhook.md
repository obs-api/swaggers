(https://developer.uber.com/docs/riders/guides/webhooks)


There are some cases where it is useful for your application to be notified of changes in a resource rather than requesting that state from the API directly. Use webhooks to track the state changes of a ride request or to get notified of the existence of a trip with the all_trips scope.

Under the application settings tab of your developer dashboard you are able to specify a webhook url, this is the URL at which your server will receive POST requests about the changes in state of resources it may be interested in.

Webhooks sent from Uber’s servers will follow a standard format so that your application can easily understand what action it may want to take based on the contents of the payload. Below are the POST parameters that can be expected with each POST request received.



Webhooks can be sent more than once and the delivery is not guaranteed to be in order. To defend against this behavior an event_id in included in the payload so the state can be managed from the client. In the case of out of order statuses, the expected behavior is to manage the state on the client and skip to the latest status. The order of ride request statuses are defined in the Requests endpoint.