Road network file format
========================

adjacentList.txt
---------------
adjacency list of the roadnetwork:

    <#_of_edges>
    <src_node_id> <dst_node_id> <length>
    <src_node_id> <dst_node_id> <length>
	...

(`length` is scaled by some parameter.)

vertexMap.txt
---------------
nodes in the roadnetwork. (each row represents a node)

    <node_id> <osm_id> <x> <y>
	...

(`x` and `y` are coordinates in a projected space based on longitude and latitude)

OSM file format
=================
 
osm_data/beijing.osm_data.txt
-----------------------------
coordinates of all osm ways

	<#_of_ways>
	<#_nodes_in_way_1> <data>
	<x> <y>
	<x> <y>
	....	
	<#_nodes_in_way_2> <data>
	<x> <y>
	<x> <y>
	....	

osm_data/beijing.waynodes.txt
-----------------------------
indices of all osm ways (each row represents a way)

	<node_id1> <node_id2> ..

osm_data/beijing.highway.txt
----------------------------
meta data of osm ways (each row represents a way)

	<way_type> <is_one_way> <name> <speed_limit>


(`speed_limit` is in km/h) 
