# EsriClusterPreview

Proof of concept to add feature cluster visualization to Esri v4 map

Primary setup:

```javascript
var options = {
    id: "flare-cluster-layer",
    clusterRenderer: renderer,
    spatialReference: new SpatialReference({
        "wkid": 4326
    }),
    singlePopupTemplate: popupTemplate,
    xPropertyName: "longitude",
    yPropertyName: "latitude",
    data: data
};

clusterLayer = new fcl.FlareClusterLayer(options);
map.add(clusterLayer);
```
