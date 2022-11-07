Added in columns to files like the name of the artist.  Also, cluster_number and km_nn9_nc3 to spotify_artists_top_tracks for futher analysis.
cluster_number is the identified connected graphs with 1 being the largest.  There were three main connected graphs.  km_nn9_nc3 is the KMeans label calculated
using the ISOMAP components.  The files in the cluster folder has more details but I only included the cluster number and KMeans label for ease of use.  
Name of the columns follows the number of neighbors and components (eg. km_nn9_nc3 -> KMean labels for 9 neighbors and 3 (ISOMAP) components).

It is important to note that the KMeans labels are only specific to each cluster.  So KMeans label of 1 for cluster 1 will not mean the same thing for KMeans
label of 1
