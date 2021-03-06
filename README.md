# `rqt_dotgraph`

Provides a ROS2 node and an rqt plugin for visualizing [DOT][dot] graph files.
You can either load a DOT file or subscribe to a ROS2 topic.

To visualize the DOT graphs, this module includes a version of [`xdot_qt.py`][xdot]
forked from [ROSPlan][rosplan] and released under [LGPLv3][lgplv3].
The forked version in this package has been modified and the changes to it are released under the LGPLv3.
The rest of this package is released under the [CC0][cc0] license.

## Nodes

### `rqt_dotgraph`

#### Subscriptions

`dot_graph` ([std_msgs/String](https://github.com/ros2/common_interfaces/blob/master/std_msgs/msg/String.msg))

* String containing the dot graph itself (e.g. the contents of a DOT file).

#### Parameters

`~title` (string, default: Dot Graph Viewer)

* Window title.

[dot]: https://en.wikipedia.org/wiki/DOT_(graph_description_language)
[xdot]: https://github.com/jrfonseca/xdot.py
[rosplan]: https://github.com/KCL-Planning/ROSPlan/blob/master/rosplan_rqt/src/rosplan_rqt/xdot_qt.py
[lgplv3]: https://www.gnu.org/licenses/lgpl-3.0.html
[cc0]: https://creativecommons.org/share-your-work/public-domain/cc0/
