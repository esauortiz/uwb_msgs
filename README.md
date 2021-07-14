# UWB ROS messages

This package includes UWB messages

AnchorInfo.msg
------------------------------------------------------------
Information related to an anchor with the following structure:

	Header header
	string child_frame_id
	string id
	bool status
	geometry_msgs/Point position
	float64[9] position_cov
	float64 distance
	float64 distance_cov
	int16 RSS

TODO: Description for each element of the message