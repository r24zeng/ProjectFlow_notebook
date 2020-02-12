# Modulity

#### Cohesion & coupling

Cohesion: a measure of coherence of module among the pieces of that module

coupling: a degree of relatedness between modules

we want semantically coherent modules.

Function relized in a module can be related by 

* topic
* interface

Good design provids clear rule on where to put new pices of code.

Examples of poor cohesion:

* coincidental cohesion -&gt; unrelated code, wrong decomposition
* god classes -&gt; too many responsibility, a function is too big need to decomposition
* control-flow cohesion -&gt; code share common control flow, eg. same value and common code but different flag to execute different function
* tempral cohesion



