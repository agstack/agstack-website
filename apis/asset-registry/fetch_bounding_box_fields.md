`Fetch Bounding Box Fields` `POST` `PRIVATE`

url: `<baseUrl>/fetch-bounding-box-fields`

Fetch the fields intersecting the _Bounding Box_
4 vertices are provided

* Headers:
> Content-Type > application/json

* Request: 
> JSON body
```
{
	"latitudes": "31.477779423633137 31.478602920901388 31.474320655972566 31.47543699178076",
	"longitudes": "74.3729835582561 74.38032208212084 74.37404571302599 74.38112674482531",
        "s2_index": "8,13,15,18,19,20"
}
```

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