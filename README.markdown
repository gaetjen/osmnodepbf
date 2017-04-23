This module helps to extract pois from osm pbf files with specified tags


Example usage
-------------

    import osmnodepbf

    foo = osmnodepbf.Parser("some.osm.pbf")

    # To see what tags are available
    tags = foo.return_tags(refresh=True)

    railways_stations = foo.parse({"railway":"station"})
    # use a set as the value to specify in more detail which nodes to select
    city_parts = parser.parse({"place": {"suburb", "borough", "quarter"}}, refresh=True)
