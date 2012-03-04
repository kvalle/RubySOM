## RubySOM

Implementation of a [Self-Organizing Map](http://en.wikipedia.org/wiki/Self_organizing_maps) (SOM) for aproximating a solution to the Traveling Salesman Problem. Written as part of a series of exercises in the course _IT3708 Subsymbolic Methods in AI_ at [NTNU](http://ntnu.no).

The problem dataset is specified in [TSPLIB format](http://www.tsp.gatech.edu/world/) as text files under `/input`, and new datasets must be added to `settings.rb` before use.
Output is generated as a series of graphs depicting the state of the SOM in each iteration.

Run as

    ruby ann.rb <task>
    
where `<task>` is one of those specified in `settings.rb`.

The implementation is discussed in our [assignment report](RubySOM/blob/master/docs/report.pdf?raw=true).

### Example: Traveling Salesman in Luxembourg

Example output from the luxembourg problem:

    ruby ann.rb luxembourg

![SOM output as animated GIF](RubySOM/raw/master/docs/lux.gif)

### Requirements

* [scruffy](scruffy.rubyforge.org) for drawing graphs
* [RMagick](rmagick.rubyforge.org) for drawing images
