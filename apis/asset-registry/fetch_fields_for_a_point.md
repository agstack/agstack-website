`Fetch fields for a Point` `POST` `PRIVATE`

url: `<baseUrl>/fetch-fields-for-a-point`

Fetch all the fields containing the point
Latitude and Longitude provided
Check for Resolution level 13 and 20
Two stage search

* Headers:
> Content-Type > application/json

* Request: 
> JSON body
```
{
	"latitude": 31.47704430446457,
	"longitude": 74.37510786779589,
        "s2_index": "8,13,15,18,19,20",
        "domain": "test.com"
}
```

> > Polygon is defined using a _Well Known Text_ (wkt) string

> > domain is an optional string, filter fields by a specific domain

> > s2_index defines which S2 index cell tokens to be returned in the response

* Response:
```
{
	"Fetched fields": [
		{
			"37d63ebdd421fb7fcb966002ea78ad1df2d4a555105eb31fe12ac7fa6f329930": {
                                "8": [ "39191" ],
				"13": [ "391905d4", "391905dc", "391905e4", "3919060c", "39190674", "3919067c" ],
				"15": [ "391905d74", "391905d7c", "391905d84", "391905d8c", ... ],
                                "18": [...],
                                "19": [...],
                                "20": [...],
                             
			}
		},
		{
			"37d63ebdd421fb7fcb966002ea78ad1df2d4a555105eb31fe12ac7fa6f329930": {
                                "8": [ "39191" ],
				"13": [ "391905d4", "391905dc", "391905e4", "3919060c", "39190674", "3919067c" ],
				"15": [ "391905d74", "391905d7c", "391905d84", "391905d8c", ... ],
                                "18": [...],
                                "19": [...],
                                "20": [...],
                             
			},
		}
	]
}
```
***