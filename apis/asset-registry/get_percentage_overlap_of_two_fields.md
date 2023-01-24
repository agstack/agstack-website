`Get percentage overlap of two Fields` `POST` `PUBLIC`

url: `<baseUrl>/get-percentage-overlap-two-fields`

Passed in 2 Geo Ids, determine what is the percentage overlap of the two fields

* Headers:
> Content-Type > application/json

* Request: 
> JSON body
```
{
	"geo_id_field_1": "7af4d1ddb9fb20e5cfe4544afab435c74e82a76024c1b8abaf9dd33163fc984b",
	"geo_id_field_2": "7b02942a48b934ed20854e9e4339be84c241c0b2770739b65c334649921a48ca"
}
```

> > Polygon is defined using a _Well Known Text_ (wkt) string

* Response:
```
{
	"Percentage Overlap": "4.943656852053799 %"
}
```
***