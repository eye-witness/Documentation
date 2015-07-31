# SOA Block Ids

Unique Block ID is a string consisting of lat/long doubled and ceil/floor. The 2 are concat with comma:

```javascript
lat = Math.ceil(lat*2).toString();
long = Math.floor(long*2).toString();
                
block_id = [lat+','+long];
```

Use split to get two elements seperated 
