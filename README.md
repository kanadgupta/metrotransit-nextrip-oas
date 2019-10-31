# Metro Transit NexTrip API Spec

This provides an [OpenAPI 3.0](https://github.com/OAI/OpenAPI-Specification) specification file for the [Metro Transit NexTrip API](https://svc.metrotransit.org/NexTrip). This spec only includes JSON responses (with XML response information coming at a later date).

## ReadMe Documentation

The OAS file in this repository is syncing to [ReadMe](https://readme.com/) via a [GitHub Action](https://github.com/marketplace/actions/readme-api-github-sync). You can view the latest ReadMe documentation [here](https://metrotransit.readme.io/reference).

## Available endpoints

| Endpoint | Description |
| :--- | :--- |
| `/Providers` | Returns a list of area Transit providers. Providers are identified in the list of Routes allowing routes to be selected for a single provider. |
| `/Routes` | Returns a list of Transit routes that are in service on the current day. |
| `/Directions/{route}` | Returns the two directions that are valid for a given route. Either North/South or East/West. The result includes text/value pair with the direction name and an ID. Directions are identified with an ID value. 1 = South, 2 = East, 3 = West, 4 = North. |
| `/Stops/{route}/{direction}` | Returns a list of Timepoint stops for the given Route/Direction. The result includes text/value pairs with the stop description and a 4 character stop (or node) identifier. |
| `/{stopid}` | This operation is used to return a list of departures scheduled for any given bus stop. A StopID is an integer value identifying any one of the many thousands of bus stops in the metro. Stop information can be derived from the GTFS schedule data updated weekly for public use. https://gisdata.mn.gov/dataset/us-mn-state-metc-trans-transit-schedule-google-fd |
| `/{route}/{direction}/{stop}` | Returns the scheduled departures for a selected route, direction and timepoint stop. |
| `/VehicleLocations/{route}` | This operation returns a list of vehicles currently in service that have recently (within 5 minutes) reported their locations. A route paramter is used to return results for the given route. Use \"0\" for the route parameter to return a list of all vehicles in service. |