 **_Jan 31, 2017: Some trajectories are missing from the repository. _**


Content
==========
* `manual_matched` : contains dense trajectories (.coor.txt) and their corresponding path on the road network (.txt) 
* `sparse_trajectories` : contains sparse trajectories (.coor.txt)
* `map` : road network and osm files


Trajectory format
==================

For files with suffix `*.coor.txt`

    <#_of_trajectories>
	<trajectory_id> <car_id> <#_of_points>
 	<timestamp> <x> <y>
	...
	<trajectory_id> <car_id> <#_of_points>
 	<timestamp> <x> <y>
	...

 Note: values in `trajectory_id`, `car_id` and `timestamp` may be placeholders

Path format
============

For files with suffix `*.txt`

Each row represents a path

	<edge_id1> <edge_id2> ...

`edge_id` references to edges in `map/adjacentList.txt`
