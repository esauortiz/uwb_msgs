# UWB ROS messages

This package includes UWB messages

## Installation
Copy this repository into your catkin workspace:

```bash
git clone https://github.com/esauortiz/uwb_msgs.git
```

Build the package

```bash
cd ~/catkin_ws
catkin_make
```

## Description

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

Where:
* ```header``` is the header of the message with message's id, time_stamp and frame_id.
* ```child_frame_id``` is the frame id placed in ```position``` in the frame_id frame
* ```id``` is the anchor's identifier
* ```status``` indicates whether the anchor is found in the network or not
* ```position``` and ```position_cov``` are the anchor's position in the frame_id frame
* ```distance``` and ```distance_cov``` are the anchor-tag distance
