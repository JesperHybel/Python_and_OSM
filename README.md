# Python_and_OSM
I have to calculate transportation time between some zones in Denmark. Specifically I want to build a multimodal urban network model using primarily Open Street Maps (OSM).
My main interest in transportation times is to calculate measures of accessibility such as job-accessibility but also accessibility to other amenities. 

Since I will be learning Python on the fly I plan to use this repository to collect bits of code solving small steps along the way. The end-goal is therefore given but I have no masterplan on how to get there so the small steps are not necessarily well structured.

I am assuming that travel demand takes the form of someone wanting to go from A to B. Given the desire to go from A to B a routing problem has to be solved to answer: How to get from A to B by travelling along the roads of the network? Naturally, this will depend on the mode of transportation be it by car, public transportation, bike or walking.

I have decided to use the package OSMnx for Python to get the roadnetwork from OSM. I have chosen OSMnx because it is well-documented and because is has automated algorithmic correction of network topology. Specifically,  

    OSMnx contributes ﬁve signiﬁcant capabilities for researchers and practitioners: ﬁrst, the automated
    downloading of political boundaries and building footprints; second, the tailored and automated downloading
    and constructing of street network data from OpenStreetMap; third, the algorithmic correction of network topol-
    ogy; fourth, the ability to save street networks to disk as shapeﬁles, GraphML, or SVG ﬁles; and ﬁfth, the ability to
    analyze street networks, including calculating routes, projecting and visualizing networks, and calculating metric
    and topological measures (Boeing 2017). 

I use Pycharm and it turns out that using conda is important for OSMnx. So my first go at installation failed because I was not aware of this. 


Boeing, Geoff (2017) OSMnx: New methods for acquiring, constructing, analyzing, and visualizing complex street networks
Computers, Environment and Urban Systems 65 pp. 126–139
