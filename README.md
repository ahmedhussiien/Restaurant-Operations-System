# Restaurant delivery system

This is a capstone project for "Data structures & Algorithms" course, written in c++ to show skills in object-oriented programming, problem solving & handling big projects.
CMUGraphics library was used provided by our educators.

### Features
- Three main order types ( Normal, VIP & Frozen ).
- Three main Motorcycles types ( Normal, Fast, Frozen ).
- Four branches. Can be increased easily.
- Delivery criteria:
  - VIP orders to be delivered first with any of the available motorcycles starting from Fast then Normal then Frozen motorcycles.
  - Frozen orders to be delivered after VIP on Frozen motorcycles only.
  - Normal orders to be delivered lastly using Normal motorcycles and Fast if there are no available Normal ones.
  - For VIP orders, orders with the highest pill or long waiting time are served first. For Normal & Frozen, orders that arrived first are served first.

- Normal orders can be promoted to VIP orders with extra money.
- Normal orders can be promoted automatically to VIP orders if it waited for more than a specified limit.
- Normal Orders can be canceled if it wasn't served.
- Motorcycles rest a specified time according to the last delivery distance.
- Each motorcycle can have different speed.
- The interface has three modes, Step by step, Interactive & Silent.
- The interface show:
  - The number of active(waiting) orders of each order type sorted where VIP are put first then Frozen and Normal.
  - The number of available motorcycles of each type.
  - Type & ID for ALL motorcycles and orders that were assigned in the last timestep. 
- All the restaurant information is to be read from a text file.
- After each session an output file will be exported that includes:
  - The number of delivered orders for each type and region sorted by it's finish time and serving time.
  - Each order waiting time, ID, serving time, arrival time and finish time.
  - Average waiting time and Average serving time.

### Technical restrictions:
- It is not allowed to use C++ STL. All data structures used must be implemented in the project.
- CMUGraphics library must be used for the interface.
