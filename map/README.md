# Collaborative map of the Shenzhen hardware ecosystem

## What?

This map is mostly focused on the electronic market for now: Huaqiangbei!

It evovles often so it would be good to have an interface that enables updates.

For example, the Shenzhai building doesn't exist anymore, but some of its weird devices can be found in other buildings.

The hope is to make this easy to use for most people, but it will take some work...



## TODO

- Test ways to make it simple to upload photos (using a form?)

- Make a form to enable uploading new points of interests? (or modifying them?)

- Test ways to validate them, and modify them.

- Test something like https://pad.land/ as a way to edit text?

- See if POIs are missing ([example](https://drive.google.com/file/d/1oq_gRsGjJA1xLqY3H1dXoxCulNS2ALuj)).



## How?

Here is an example to add a new map pin with 2 images (see the html file):

    {
        position: [114.085413, 22.544441],
        title: "Huaqiangbei",
        images: ["/assets/image1.jpg", "/assets/image2.jpg"]
    },

Extra:

- An "address" field can be added (and potentially be misused to add comments)

- An "anchor" or "labelOffset" field can also be added to place the label differently (see html file)



## History

This map exists thanks to other repos/lists, including these:

- https://github.com/samyk/ScalableHCI.github.io/blob/map-images/map.html

- https://github.com/ScalableHCI/ScalableHCI.github.io/blob/main/map.html

- https://github.com/ScalableHCI/HQB-map

- https://dangerousprototypes.com/docs/File:Hqb-map-front.png


