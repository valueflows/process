# vf:InputOrOutput

a slot which accommodates resources going into the process or going out of the process

[N-ary Relation](https://www.w3.org/TR/swbp-n-aryRelations/)

## Object Properties
(relationships)

### vf:resource
relates input/output to a resource

### vf:action
relates input/output to a verb (explained below)

(reverse)
### vf:io
relates process to a input/output

## Data Properties

## Actions

### consume
for example an ingredient composed into the output, after the process the ingredient is gone

resource effect: increment *vf:quantity* of affected resource by value of *vf:affectedQuantity* in event

### assemble

resource effect: create *vf:hasComponent* relationship between resource referenced from event with *vf:assembledInto* property and the affected resource & unset *vf:currentLocation* of affected resource

### receive

### load
specific for [vf:Transportation](https://github.com/valueflows/process/blob/master/Transportation.md), transported resource enters the process

resource effect: unset *vf:currentLocation* of affected resource

### accept
in processes like repair or maintentance, same resource will appear in [vf:Output](https://github.com/valueflows/process/blob/master/Output.md) with *improve* verb

### use
for example a tool used in process, after the process, the tool still exists

### work
labor power towards a process

### cite
for example a design file, neither used nor consumed, the file remains available at all times



### produce

a new resource produced in that process

resource effect: increment *vf:quantity* of affected resource by value of *vf:affectedQuantity* in event

### disassemble

resource effect: remove *vf:hasComponent* relationship between resource referenced from event with *vf:assembledInto* property and the affected resource & set *vf:currentLocation* of affected resource to value of *vf:currentLocation* of resource which had *vf:hasComponent* relationship with it.

### issue

### improve
in processes like repair or maintentance, same resource will appear in [vf:Input](https://github.com/valueflows/process/blob/master/Input.md) with *accept* verb
 
### unload
specific for [vf:Transportation](https://github.com/valueflows/process/blob/master/Transportation.md), transported resource leaves the process

resource effect: set *vf:currentLocation* of affected resource to value of *vf:atLocation* in event

## Phases
Input or Output doesn't change from one phase to another, each phase has distinct input/output with relationships to relevant input/output in other phases.

* Recipe - often containing broad description of acceptable resources
* Plan - in this stage one can narrow further acceptable inputs from Recipe and serve as foundation to cast an Intent
* Alocation - in this stage one has agreement for particular resource to bind with input slot
* Event - stage after running the process which refers to resource actually put into input slot

## Examples

**TODO**
