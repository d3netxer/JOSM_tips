You can make OSM queries at http://overpass-turbo.eu/ and extract your results in various forms, including bringing them into JOSM for further editing.

Here is an example. During the HOT Nepal Crisis response, a project was being set up that would update IDP sites in central Kathmandu. The tagging schema was being defined, and this would involve making some changes to the existing tags that were created for the initial project. All IDP sites would need their source tag changed and a new status tag added to them.

The first step was querying in overpass turbo to get all IDP sites in central Kathmandu. Here is the query used:

```
/*
idp camps kathmandu
*/
[out:xml][timeout:120];
way[~"idp:"~"spontaneous_camp"]({{bbox}});
// print results
out meta;
>;
out meta;
```

The data was then loaded into JOSM. 

Windows: tag, filter, selection

The filter window was turned on and the filter string was entered: Pleiades 2015-04-27, CNES, Airbus DS

drag mouse and select all objects. nodes will be selected too, but you don't want to add tags to the individual nodes. 
On selection window click Search and add this string: selected type:way (replace action)

You will be able to see all the tags in the tag window. You can double click the tag to modify a tag or add a new one. Be aware that there might be multiple values for a particular key. This might involve digging into the feature set to make some corrections before modifying all of the tags at once.

This also was a good opportunity to do validation.

