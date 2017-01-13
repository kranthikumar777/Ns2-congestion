# Ns2-congestion
ECEN 602 Network Simulation Assignment 02
Implementing a small network in Ns2
----------------------------------------------------------
Team Number:23
Member 1: Kranthi Kumar Katam  (UIN: 225009204)
Member 2: Matthew Roe          (UIN: 321007055)
Member 3: Jifang Mu            (UIN: 821005313)
----------------------------------------------------------
The package contains 3 files :
1. ns2.tcl 
2. report
3. readme.txt
----------------------------------------------------------
Design:
1. Establish appropriate links (duplex) with DROPTAIL and RED queue mechanism
2. Create TCP agents and attach it to H1 and H2, UDP agents to H6
3. Add FTP traffic source over these TCP agents, and CBR traffic over UDP agents
4. Create two TCP sinks and attach them to H3 and H4, UDP sink to H5
5. Record the instantaneous throughput for each stream
6. Record the overall throughput for each stream and output this quantity
7. Graph the instantaneous throughput over time (results in trace file from 5) using xgraph
------------------------------------------------------------
Implementation:
1. In the command line open the directory where you have saved the file.
2. Use the following command line to execute ns2.tcl
     ns ns2.tcl <QUEUE_MECHANISM> <SCENARIO_NO>
     where <QUEUE_MECHANISM>  can be either of { DROPTAIL, RED }
     <SCENARIO_NO> can be either of { 1, 2 }
------------------------------------------------------------
Summary:
This code will simulate the network provided in the two scenarios, one with two TCP 
streams only and the other with two TCP streams and one UDP stream. These two scenarios can be tested 
for both DROPTAIL and RED queueing mechanisms. This program tests the above scenarios and can provide
insight into the differences between DROPTAIL and RED while also showing the effects of massive UDP traffic 
on each of the queuing mechanisms. 
