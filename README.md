# Message Oriented JavaScript Framework (mojafe)
Exploration in progress. Basic idea is to define a framework that is based purely on modern HTML and JavaScript. Part of the goal is to provide a framework that doesn't require any files to be downloaded or installed but also doesn't preclude using other JavaScript libraries if desired.

## Application Architecture
![](/mojafe.png)

|Application Component|Description|
|---------------------|-----------|
|Component            |Encapsulates a discrete aspect of an application. Internally the component uses an model-view-controller (MVC) pattern to manage the view logic, trigger command events, and handle response events|
|Service              |Encapsulates reusable logic not related to components. 
|Command Channel      |Used by components to send "commands" (i.e. command events) to services|
|Response Channel     |Used by components to receive "responses" to commands|
|Layout               |Initializes the placement of components in the application|
|Router               |Manages component view state via response events|

