## Getting GeoJSON data from OSM

Using Overpass API: http://overpass-turbo.eu/

    <osm-script>
      <query type="relation">
        <has-kv k="name" v="Great Divide Mountain Bike Route"/>
      </query>
      <!-- added by auto repair -->
      <union>
        <item/>
        <recurse type="down"/>
      </union>
      <!-- end of auto repair -->
      <print/>
    </osm-script>