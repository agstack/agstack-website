`Fetch Overlapping Fields` `POST` `Private`

url: `<baseUrl>/fetch-overlapping-fields`

Fetch the overlapping fields for a certain threshold, returning the field’s geo json.

* Headers:
> Content-Type > application/json

* Request: 
> JSON body
```
{
	"wkt": "POLYGON ((74.35855950604382 31.479723509875665,74.36619843731823 31.473830840390207,74.37044705639782 31.47968691058925,74.35855950604382 31.479723509875665))",
	"resolution_level": 13,
	"threshold": 90,
	"domain": "test.com"
}
```

> > Polygon is defined using a _Well Known Text_ (wkt) string

> > domain is an optional string, filter fields by a specific domain
> 
* Response:
```
{
	"GEO Ids": [ "da2504ff0e16a77ad5d86d0c4bd6f21fcd33c69ce78cb6c03d0245ab719c22b5"],
	"Message": "The field Geo Ids with percentage match of the given threshold."
}
```
***
