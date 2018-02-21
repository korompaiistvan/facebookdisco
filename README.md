# facebookdisco
A 2018.02.21-én budapesti Pecha Kucha rendezvényen előadott adataelemzés forrásai

### Message charts:
To download your Facebook archive, go to Settings and choose Download a copy of your Facebook data.
This will (after some time) give you with a static html dump, from which you can parse the messages into a single csv using the 'Parse messages.ipynb' Jupyter notebook.

Connect to this csv with the tableau workbook to gain access to the charts.

### Network viz:
To download the data for the graph, install Lost Circles from https://lostcircles.com/. This will allow you to download your friends' network after a load of roughly an hour or so (depending on your number of friends, their connections and your machine/network speed).
(You'll need to change your Facebook language to English before you start loading)
##### The network visualization was done in Gephi
Download the graphml from the Lost Circles extension and open it with Gephi.
Use ForceAtlas2 for the layout.
Run Network Diameter statistics to calculate Betweenness. 
Run Modularity statistics to automatically detect communities.

Size nodes by Betweenness and color them by Modularity class.

Render your view in Preview and enjoy!
