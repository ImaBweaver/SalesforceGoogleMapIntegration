# SalesforceGoogleMapIntegration
Code to implement the google maps integration onto the salesforce opportunity page

This code requires some fields and custom objects. The only custom object required is a Site object. This object holds information including the site address, geo-coordinates, and distance/time calculations. Holding this information helps to reduce the number of API calls that need to be made to google maps.

This was origianlly programed to parse the JSON response as a string, but I am working on getting it parsed as it's own object. The objective of this is to get the directions to pull into their own object, so I can then map them on the screen for the viewer. More on this to come.

Anyway, feel free to tool around and make any updates you need to.

Thanks,
Brandon Weaver
