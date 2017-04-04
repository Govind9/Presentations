<link rel="stylesheet" href="css/theme/mandeep.css" id="theme">
>### Multi-Threaded Geometric Rendering

----

*Presented By*

**Amarjeet Singh Kapoor**

**Govind Sharma**

---

>##### Acknowledgements

* Amanpreet Singh Brar (Project Guide)
* Marius Kintel (Creator of OpenSCAD)
* Torsten Paul (Developer at OpenSCAD)

---

#### OpenSCAD

* OpenSCAD is a free and Open-source software application for creating solid 3d CAD objects.
* It is a script only based modeler, with a specific declarative and functional language.

----

#### OpenSCAD is Awesome!

* It is a popular CAD software with millions of users worldwide.
* With Some Companies based on It.
* It is also taught in many institutes around the world as part of their academic curriculam.
* It has an on line community of around a hundred contributers and many many users.

---

#### Project Inspiration

* To complete a project that has actual real life usage and need.
* To work in an open source community.
* To solve issues that are not self made and require studying code written by many experienced people.

---

#### Central Issues

OpenSCAD community was the perfect match for finding a project matching our expectations. Following are the major issues that we focused on during our project:

----

#### Multi-threading the geometric rendering

* One of the high priority tasks in OpenSCAD GSoC project list.
* Demands utilization of resources efficiently during the cpu intensive rendering processes.
* Requires understanding multi threading, parallelization and safety issues during concurrency.

----

#### Halting an ongoing render process

* Rendering consumes a lot of time, specially on big models.
* There was no mechanism to stop an ongoing render process.
* Can be frustrating when rendering button is pressed unintentionally.
* Requires understanding exception handling, message passing and design patterns in OOPs.

----

#### Generalized progress widget

* The progress widget shows the progress of each render process.
* Incorporates the cancel button.
* Needs to be generalized for ease of coding.

----

#### RootTag search, storage and management

* Mechanism for partial evaluation of node tree.
* Multiple nodes can be marked as root nodes for partial evaluation.
* Warning mechanism needed to notify the user of multiple root tagged nodes in the tree.

---

#### Solution Strategies

* Multi threading can be done by creating new threads at each branch encountered in the tree.
* Halting can done properly using the progress report function in CGAL render processes.

----

* To Generalize it could be shifted to super visitor class
* Recursive lambda function (functor) is used to search and store nodes with RootTags in the node tree.

---

#### Advantages over previous versions

* The multi-threading will help make software Responsive, use resources efficiently and reduce CPU idle time during renders.
* Halting mechanism will allow tackle unintentional rendering attempts.

----

* Generalized progress widget will ensure ease of coding in future features and reduce redundancy.
* Using lambda function improves performance significantly while also adding warning mechanism to the searching function for RootTags.

---

### Thank You

