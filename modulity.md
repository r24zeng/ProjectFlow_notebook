# Modulity

#### Cohesion & coupling

Cohesion: a measure of coherence of module among the pieces of that module

coupling: a degree of relatedness between modules

we want semantically coherent modules.

Function realized in a module can be related by 

* topic
* interface

Good design provides clear rule on where to put new pices of code.

Examples of poor cohesion:

* coincidental cohesion -&gt; unrelated code, wrong decomposition
* god classes -&gt; too many responsibility, a function is too big need to decomposition. It's many unrelated functions.
* control-flow cohesion -&gt; code share common control flow, eg. same value and common code but different flag to execute different function. So merge the pices results in bad complicated and may not related cohesion. It's a only a function.
* tempral cohesion



#### coupling:

 It is induced by different types of dependencies among modules 😅 . eg. If you care the data from where, the two modules are coupling. If you put them acturally as one module, it saves the communication, minimize the decomposition, minimize the strength of the dependency.

* data -- A provides data to B, weakest dependency
* control -- A controls the execution of B
* source -- A calls a service from B
* identity -- A is aware of identity of B
* location -- A is aware of location of B
* quality of service -- A expects certain QoS from B \(eg, ecpect B comes 10 am\)
* hidden coupling \(bad\) can be avoided by making explicit interfaces \(global variable, relocation\)

implementation inheritance -&gt; strong coupling, bad, decompiste inheritance to interface

* eg, superclass contains subfunctions, and subfunctions can be reused. Prefer interface inherence.

Control coupling should be avoided

stamp coupling should be avoided -&gt; more data is passed to a module which not necessary, only pass data necessary to perform the function, security reson, independency policy

low coupling is good: we want to use module data coupling. No coupling is best, but data coupling is second good.





