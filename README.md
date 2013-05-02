Contact Recaster
===============

Introduction
------------

We are releasing this easy to use code for any user who does not want to REdo mobility experiments to change mobility parameters (transmission range, beaconing period, loss tolerance), but still want to get realiable mobility traces for other different parameters.

Background
------------

The Contact Recaster takes mobility traces (in One format) from real experiments or synthetic models and rewrite this trace in as many traces as the user specifies.

The Contact Recaster allows for a given mobility trace to change 

    < Transmission range > is defined as the maximum distance at which a node can see other nodes 
    < Beaconning-period  > is defined as the time frequency to use for checking if nodes are in contacts with each other 
    <   Loss-tolerance   > is defined as the maximum lost beacons allowed

Building
------------

Two possibilities:


(1) If you want to run the whole system, rely on https://github.com/neush/ditl to build all the needs.
    
(2) If you already have a mobility trace (Format One) you can directly go to the Run part.

NB: if you have a mobility trace in ns2 you can use The DynamIc Trace Library (ditl) to convert your ns2 trace in format One trace, in that case you need to follow th elink given in (1).


Run
------------

First download the source code 
