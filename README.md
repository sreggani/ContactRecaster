Contact Recaster
===============

Introduction
------------

We are releasing this easy to use code for any user who does not want to REdo mobility experiments to change mobility parameters (transmission range, beaconing period, loss tolerance), but still want to get realiable mobility traces for other different parameters.

Background
------------

The Contact Recaster takes mobility traces (in One format) from real experiments or synthetic models and rewrite this trace in as many traces as the user specifies.

The Contact Recaster needs to know the maximum number of nodes participating in the experiment and allows for a given mobility trace to change: 

    < Transmission range > is defined as the maximum distance at which a node can see other nodes 
    < Beaconning-period  > is defined as the time frequency to use for checking if nodes are in contacts with each other 
    <   Loss-tolerance   > is defined as the maximum number of lost beacons allowed
    <   %beacons lost     > is defined as the percentage of lost beacons from the whole mobility trace
    
    WARNING: this parameter is not yet integrated into the code even if it will appear in the name of teh final    
    rewritten trace

Building
------------

Two possibilities:


(1) If you want to run the whole system, rely on https://github.com/neush/ditl to build all the needs.
    
(2) If you already have a mobility trace (Format One) you can directly go to the Run part.

NB: if you have a mobility trace in ns2 you can use The DynamIc Trace Library (ditl) to convert your ns2 trace in format One trace, in that case you need to follow th elink given in (1).


Run
------------

First download the source code here.

Example: 
To rewrite a contact trace named "CTrace" checking each (Beaconning-period) 2 seconds using a (%beacons lost is set to 0 for now), Transmission range of 10M, tolerating a loss of 2 beacons, and a maximum number of nodes of 19, do

        sh ContactCaster CTrace 2 0 10 2 19 > log

You can then check you result in FinalContactTrace_2_0_10. In case of any wanderings about the steps you can chack the correspodant 'log'
