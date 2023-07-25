
# Format

Models in this file will be defined in psuedo json such that
`field: Type | format`
where format is an example of a value or additional notes

Two pipes (`|`) indicates that a field MUST be of one of the provided values

## Video
### VideoDescriptor
```json
{
    title: String,
    duration: UInt | Number of seconds,
}
