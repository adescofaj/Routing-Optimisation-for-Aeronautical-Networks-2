# Routing-Optimisation-for-Aeronautical-Networks-2
In this assignment, you will address a real-world problem of routing optimisation for aeronautical networks. Thousands of aeroplanes fly over the North Atlantic every day. In order to provide Internet access to passengers onboard, each aeroplane needs to find an optimal data packet routing path to a ground station (GS) in terms of one or two more objectives to be optimized.


In order to find an optimal data packet routing path, there are two metrics to be considered, end-to-end data transmission
rate and end-to-end latency.

The end-to-end latency is the sum of all delays imposed by each link. For example, a routing path is: 
Airplane-5 --> Airplane-3 --> GS-1

The delay imposed by each link is 30 milliseconds (ms). So, the end-to-end latency of the routing path:
Airplane-5 --> Airplane-3 --> GS-1 = 60 ms

The end-to-end data transmission rate is the minimum transmission rate of each link in the routing path. For example, a
routing path is:
Airplane-5 --> Airplane-3 --> GS-1

The data transmission rate between Airplane-5 and Airplane-3 is 52.857 Mbps, and the data transmission rate between
Airplane-3 and GS-1 is 43.505 Mbps, then the end-to-end data transmission rate of the routing path
Airplane-5 --> Airplane-3 --> GS-1 = 43.505 Mbps

Explicitly, a link’s transmission rate is determined by the distance of a pair of communicating aeroplanes. When the distance between two nodes (aircraft) is longer than 740 km, we will assume there is no communication link, say the transmission rate will be 0 Mbps. For example, if the distance between Airplane-5 and
Airplane-3 is 380 km, so 350 km < 380 km <= 550 km the data transmission rate of the link between Airplane-5 and
Airplane-3 will be 11.023 Mbps.

Optimisation problems
There are two problems you should address:
1. Single-objective optimisation. There are three GSs that an airplane can access it to access the Internet. The
three GSs are deployed at Heathrow airport (LHR) (Latitude, Longitude, Altitude) = (51.4700° N, 0.4543° W, 81.73
feet), Narsarsuaq airport (UAK) (Latitude, Longitude, Altitude) = (61.9000° N, 41.25° W, 112.73 feet), and Newark
Liberty International Airport (EWR) (Latitude, Longitude, Altitude) = (40.6895° N, 74.1745° W, 8.72 feet). Find a
routing path having a minimum end-to-end latency for each airplane that can access any of the above-mentioned
GS, either at Heathrow airport (Latitude, Longitude, Altitude) = (51.4700° N, 0.4543° W, 81.73 feet) or Newark
Liberty International Airport (Latitude, Longitude, Altitude) = (40.6895° N, 74.1745° W, 8.72 feet), or Narsarsuaq
airport (UAK) (Latitude, Longitude, Altitude) = (61.9000° N, 41.25° W, 112.73 feet). There is no other constraint
imposed.
2. Single-objective optimisation. There are three GSs that an airplane can access it to access the Internet. The
three GSs are deployed at Heathrow airport (LHR) (Latitude, Longitude, Altitude) = (51.4700° N, 0.4543° W, 81.73
feet), Narsarsuaq airport (UAK) (Latitude, Longitude, Altitude) = (61.9000° N, 41.25° W, 112.73 feet), and Newark
Liberty International Airport (EWR) (Latitude, Longitude, Altitude) = (40.6895° N, 74.1745° W, 8.72 feet). Find a
routing path having the maximum end-to-end data transmission rate for each airplane that can access a GS
deployed at the above-mentioned three GSs with the constraints of:

1. The total number of relay nodes is less than 4 for each airplane that wants to access a GS.
2. Each airplane can only act as a relay node no more 5 times.
