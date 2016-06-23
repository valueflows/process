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

## Verbs

### Input
* use - for example a tool used in process, after the process, the tool still exists
* consume - for example an ingredient composed into the output, after the process the ingredient is gone
* cite - for example a design file, neither used nor consumed, the file remains available at all times
* work - labor power towards a process
* accept - in processes like repair or maintentance, same resource will appear in [vf:Output](https://github.com/valueflows/process/blob/master/Output.md) with *improve* verb
* load - specific for [vf:Transportation](https://github.com/valueflows/process/blob/master/Transportation.md), transported resource enters the process

### Output

* create - new resource created in that process
* improve - in processes like repair or maintentance, same resource will appear in [vf:Input](https://github.com/valueflows/process/blob/master/Input.md) with *accept* verb
* unload - specific for [vf:Transportation](https://github.com/valueflows/process/blob/master/Transportation.md), transported resource leaves the process

## Phases
Input or Output doesn't change from one phase to another, each phase has distinct input/output with relationships to relevant input/output in other phases.

* Recipe - often containing broad description of acceptable resources
* Plan - in this stage one can narrow further acceptable inputs from Recipe and serve as foundation to cast an Intent
* Commitment - in this stage one has agreement for particular resource to bind with input slot
* Event - stage after running the process which refers to resource actually put into input slot

## Examples

**TODO**
