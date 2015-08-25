# Process vocab

This is separated out from the [OVN vocab](https://github.com/openvocab/ovn), of which it is a component. See also the [Principles](https://github.com/openvocab/ovn/wiki/Principles-for-this-vocabulary) for the OVN vocab, which are also the principles for this one.

## Why?

We know of two different projects that use Process in compatible ways, and are interested in collaborating. We hope more will come.

## Who uses this?

So far, [NRP](https://github.com/valnet/valuenetwork) and [IPOTables](http://ipotables.net/). And you?

## Overview of Processes

By Process, we mean an activity that transforms inputs into outputs. The outputs might then become inputs to other processes, forming networks and chains. Those chains may be circular, where an output from one process becomes an input to another process that occurred previously in the same chain.

For example: a farming process takes compost, soil, seeds, water and human and mechanical work as inputs, and transforms them into grains, nuts, fruit, and vegetables. Those ingredients may go to kitchens that create dinners for people to eat. Some of those ingredients may be pared off in preparation, or spoil, or be left on plates. Those leftovers go into compost, which starts the process chain over from the beginning.

Or for a bad example: a CAFO (Confined Animal Feeding Operation) produces a lot of manure. They put manure into big lagoons, which drain into the water table, and come back up in people's drinking water, causing diseases, for which the people become inputs to a hospital.

One of the inputs to the CAFO process is antibiotics. The animals are filled with antibiotics because they get sick in the CAFO environment. And the antibiotics are also an output, mixed in with the manure.

The antibiotics then breed resistant bacteria, which end up in hospitals, killing the people, because the common antibiotics no longer work.

## Pictures!

This is the NRP view of processes, which occur in resource flow networks, and live in three layers: Recipes, which describe how processes work. Plans, which describe processes which are intended to happen. And Reality, which is a record of processes that have already happened.

![process resource flow](https://i.imgur.com/74gIY5C.png)

This is the IPOTables view of processes. The idea in the center of IPO is to take the simple standard of the IPO Model – Input, Process, Output – that is widely used in system-analysis and life cycle assessment (LCA)/eco-management (e.g. ISO 14040) and bring it to the world of open-source-hardware documentation. In life-cycle-assessment complex production processes are broken down in simpler and manageable steps – modules. Every module has 1) INPUTS like materials, components & energy, 2) PROCESSES that transform inputs into outputs and 3) OUTPUTS like products and byproducts. I-P-O modules. Listing all outputs makes waste visible and is a pre-step to connect outputs to input-sides, to connect modules to chains (and maybe circles).

![](http://ipotables.net/wp-content/uploads/2014/09/dg-56p.png)

I-P-O documentation helps to monitor, communicate and connect flows of energy, materials, components and (by)products.

## Goal

The goal of this process is to take these inputs (NRP, IPOTables, and any other projects that want to join) and create a common vocabulary that brings them together.



