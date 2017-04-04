###Multi-Threaded Geometric Rendering
*Presented By*

**Amarjeet Singh Kapoor**

**Govind Sharma**

---

#####Acknowledgements
* Amanpreet Singh Brar (Project Guide)
* Marius Kintel (Creator of OpenSCAD)
* Torsten Paul (Developer at OpenSCAD)

---

####OpenSCAD
* OpenSCAD is a free and Open-source software application for creating solid 3d CAD objects.
* It is under the umbrella organization of BRL-CAD.
* It is a script only based modeler, with a specific description language.

----

####OpenSCAD is Awesome!
* It is a popular CAD software with millions of users worldwide.
* It has an online community of around a hundred contributers and many many users.
* It is also taught in many institutes around the world as part of their academic curriculam for civil engineers and designers alike.

---

####Project Inspiration

* To complete a project that has actuall real life usage and need.
* To work in an open source community.
* To solve issues that are not self made and require studying code written by many experienced people.

---

####Central Issues
OpenSCAD community was the perfect match for finding a project matching our expectations. Following are the major issues that we focussed on during our project:

----

####Multi-threading the geometric rendering
* One of the high priority tasks in OpenSCAD GSoC project list.
* Demands utilisation of multiple processor cores during the cpu intensive rendering proceses.
* Requires understanding multithreading, parralelisation and safety issues during concurrency.
* Handling thread-Unsafe libraries like CGAL.

----

####Halting an ongoing render process
* Rendering consumes a lot of time, specially on big models.
* There was no mechanism to stop an ongoing render process.
* Can be frustrating when rendering button is pressed unintentionally.
* Requires understanding exception handling and message passing design patterns in object oriented programming.
* Processed nodes must be cached to save time in consecutive renders.

----

####Generalized progress widget
* The progress widget shows the progress of each render process.
* Incorporates the cancel button.
* Needs to be generalized for ease of coding.

----

####RootTag search, storage and management
* Mechanism for partial evaluation of node tree.
* Multiple nodes can be marked as root nodes for partial evaluation.
* Warning mechanis needed to notify the user of multiple root tagged nodes in the tree.

---

####Solution Stratergies
* Multithreading can be done by creating new threads at each branch encountered in the tree.
* Halting can done properly using the progress report function in CGAL render processes.
* Recursive lambda function is used to search and store nodes with RootTags in the node tree.

---

####Advantages over previous versions
* The multithreading will help the software save time, use resources efficiently and reduce cpu idle time during renders.
* Halting mechanism will allow tackle unintentional rendering attempts.
* Generalised progress widget will ensure ease of coding in future features.* Using lambda function improves performance significantly while also adding warning mechanism to the searching function for RootTags.

---

###ThankYou
