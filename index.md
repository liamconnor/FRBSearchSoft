## Benchmarking FRB Search Software

* Date: February 21, 2019 
* Time: 9:30 - 17:00
* Location: University of Amsterdam

### People involved
* Joeri van Leeuwen (ASTRON, Dwingeloo, the Netherlands)
* Liam Connor (University of Amsterdam, Amsterdam, the Netherlands)
* Alessio Sclocco (Netherlands eScience Center, Amsterdam, the Netherlands)
* Adriënne Mendrik (Netherlands eScience Center, Amsterdam, the Netherlands) 
* Annette Langedijk (SURF, Utrecht, the Netherlands) 
* [*Please add your name*]

### Workshop program
* Opening by Liam Connor (University of Amsterdam, Amsterdam, the Netherlands)
* Talk by Adriënne Mendrik (Netherlands eScience Center, Amsterdam, the Netherlands) “Introduction to Challenges and the EYRA Benchmark Platform” [(slides are here)](https://github.com/EYRA-Benchmark/FRBSearchSoft/blob/master/FRB%20Benchmark%20Workshop%20-%20Adrienne%20Mendrik%20(eScience%20center)%20.pdf)
* Liam Connor (University of Amsterdam) “Introduction to the FRB Detection Benchmark Initiative”
* Coffee Break
* Brainstorm on the FRB Detection Benchmark:
  * Input: Filterbank (.fil) or other
  * Output: Text file
    * What should be in there? SN, dispersion, pulse width, arrival time, scattering measure, ...
    * How should it be structured?
  * Benchmark data: 
    * Different telescopes (what data can people contribute? How large?)
    * Simulation of the FRBs
  * What metrics should be used to rank the algorithms?
* Lunch Break
* Break-out sessions
  * Dockerize software
  * Design Benchmark (data, simulations, metrics, etc)
* Closing

Potential deliverables:
* Global benchmark design and an overview of existing data
* Some dockerized software packages

## Notes

* It would be great to be able to include different components as well, instead of a whole pipeline (for example AstroAccelarate does only one part and is not a complete pipeline). It would be nice to see how different components mix and match
* We should discuss and agree on interfaces (what is fed into the software), is it possible to have a layer of abstraction? Cheeta is providing something like that. Would be interesting to discuss this further. Maybe separate workshop?
* Next to benchmarking, unit tests would be very helpful as well. Maybe look at the continuous benchmarking, example from the medical image analysis field: https://continuousregistration.grand-challenge.org/
* Which simulations to inject? Maybe try different ones?
* We should take into account that there is a danger that you are overtuning your software for the simulations, maybe also test on real data? With observer study (astronomers) as a next step?
* Make an overview of all search and injection codes
* Unit tests would be great. If you change something to the code, are FRBs still found (that’s what would be great to have). 
* Evaluation: Use a confusion matrix or ROC curve for each region of parameter space?
* Ccp4 uk initiative (http://www.ccp4.ac.uk/), collaborative computational project in a different field, could be used as an example. 
* Maybe later, add more data to improve the frb detection software, like lightning data etc
* Maybe start easy with Gaussian data and inject pulses. Focus only on accuracy? Or also speed?


