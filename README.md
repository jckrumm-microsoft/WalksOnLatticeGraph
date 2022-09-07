# Statistics for all walks of a given length on a lattice graph

Please see the accompanying paper at ...

# Files visit_counts_T{}.csv

For a walk of length/duration T, these files give counts and probabilities for visiting an (x,y) cell on a walk on a lattice grid, starting at (0,0). The columns are:

* XEnd - x coordinate of the vertex/cell at the end of the walk
* YEnd - y coordinate of the vertex/cell at the end of the walk
* T - length/duration of the walk. This is the total number of moves made along edges in the lattice graph.
* WalksToEndCount - the number of distinct possible walks from (0,0) to (x,y) of length/duration T
* XVisit - x coordinate of the visited vertex/cell
* YVisit - y coordinate of the visited vertex/cell
* VisitsToXYVisitCount - the number of walks that visit the vertex/cell at (XVisit,YVisit)
* VisitToXYVisitProbability - out of all the walks, the probability that a randomly chosen walk visits (XVisit,YVisit). Computed as VisitsToXYVisitCount/WalksToEnd.

# Files dwell_counts_T{}.csv

For a walk of length/duration T, these files give counts and probabilities for dwelling at an (x,y) cell on a walk on a lattice grid, starting at (0,0). The columns are:

* XEnd - x coordinate of the vertex/cell at the end of the walk
* YEnd - y coordinate of the vertex/cell at the end of the walk
* T - length/duration of the walk. This is the total number of moves made along edges in the lattice graph.
* WalksToEndCount - the number of distinct possible walks from (0,0) to (x,y) of length/duration T
* XVisit - x coordinate of the visited vertex/cell
* YVisit - y coordinate of the visited vertex/cell
* VisitsToXYVisitCount - the number of walks that visit the vertex/cell at (XVisit,YVisit)
* DwellVisitXYDuration - duration of visit
* DwellVisitXYDurationCount - the number of walks that visit the vertex/cell at (XVisit,YVisit) that dwell here for DwellVisitXYDuration
* DwellVisitXYDurationProbabilityGivenVisit - given a visit to this vertex/cell, the probability that the visit has a duration of DwellVisitXYDuration. Computed as DwellVisitXYDurationCount/VisitsToXYVisitCount
