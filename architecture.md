# Architecture and design

#### Design

plan/solution to how to satisfy requirements

#### Leverl of design

1. high level design\(aka architectural design\): main system components and their connections
2. detailed design - details such as algorithm selection , detail API design ……\(allow to write code\)

#### subject of design

1. software design - architecture + detailed design as it relates to code
2. end - user interface design - usability + esthetics 

#### Architecture:

1. components + connections: Join happens, think about how components communicate with each other.
2. often represented using nultiple views: It's good that different people work on different specifications
3. now responsibilities assigned to developers

#### Design process

1. Design criterion: function requirements and quality requirements. 
2. Design loop: generalize ideas, analysize design criterion, make decision, optimization.

#### Avarage exercise

1. store running sum of numbsers+count, return total divided by count
2. Take average of pairs of numbers then recursively averages of result pairs
3. Divide each number by the count and add 
4. split into subsets, solve subproblems , aggregate 
5. store entire input then caculate on demand

#### Design loop

1. systemsis \(generate ideas\), brain stroming, iterative reaserch, experience
2. conceptualize design ideas,descrption, prototyle, simulation
3. analyze, evaluate what requirements and design criteria
4. decision making, trade off resolved.

#### Design contian:

Fitteness for purpose: functionality, runime perfermance, reliability, security, ……

fiterness for futhure: Modifiability, extensibility, maintainability，……

#### Maintenance:

repairs -&gt; removing reperted faults \(corrective maintenance\) + discovery and removal of dormant fualts\(preventative maintenance\)

modifications -&gt; new features\(extension\) + adjusted to environment changes\(adaptive maintenance\)

#### Modifiability:

functional modify quality 

**module** is a unit of system decomposition with how well define purpose and interface. module has relationship with environment\(other modules and other system you need to talk to, context\)+ provide interface\(functions provided to the environment\) + gurantee properties\(call the function, the module works properly\) + required interface\(module reqired from environment\) + environment guarantees\(precondition you need to be set up\) + environment properties.

**interface** is a contract between the module and the environment. contract means two way-promise, do the job for someone and someone pay you. We hope interface is successful and also good perfermance. 

**syntactical aspect interface** is about How to call it. Be detail: function service signatures\(function names, number of types or parameters\), also protocols\(data formating, ordering of calls\)

**semantical aspect interface** is about what it does. effects of calling a function\( how to modify , per/pos-condition, random performance aspects, reliability\)

#### Example of function name:

File Handle open\(string name\): This is function signature and also minly **syntactic**\(except for the evocative names\). **Semantics**: Add a desciption of what it does would give the semantics. error codes\(understand what condition\). response time. **protocol:** fixed sturcture of function such as English grammar \(this is also syntactic part\).

#### Module implementation\(secrets\):

what are good secrets\(hide latency, cache data\), representation of data, properties of devices\(hardware, mechanism the support policies\(hide how you done\), implementation of world model data\(how to organize on georaphical map\)

#### uses of modelization:

* help with system comprehension\(understand interface of module to know big picture\)
* paralle develops\(various teams allow you to organize the work\)
* support evoluation\(limits ripple effects\)
*  reuse of modules
* tesing\(write test to each unit and easy anlyze the error\)









