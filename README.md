# SalesforceGoogleMapIntegration
Code to implement the google maps integration onto the salesforce opportunity page

This code requires some fields and custom objects. The only custom object required is a Site object. This object holds information including the site address, geo-coordinates, and distance/time calculations. Holding this information helps to reduce the number of API calls that need to be made to google maps.

This was origianlly programed to parse the JSON response as a string, but I am working on getting it parsed as it's own object. The objective of this is to get the directions to pull into their own object, so I can then map them on the screen for the viewer. More on this to come.

The order of the code is as follows:

Component - Shows the UI on the main salesforce screen. Makes calls to the Client-Side Controller
Client-Side Controller - Talks between the server-side controller and the component. To fetch things from the database, the Client-Side controller must call the server-side controller and pass the value to the component (or vice versa for the UI to write to the database)
Style - sets style elements that can be used by the component to add different formats to the UI
Server-Side Controller - Performs most of the operative heavy lifting. It gets values from the client-side controller, does the operation, and returns the value. There are multiple functions in this server-side controller that do different things.

Anyway, feel free to tool around and make any updates you need to.

Thanks,
Brandon Weaver
