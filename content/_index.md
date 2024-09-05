+++

title = "An Aggregate Vascular Morphogenesis Controller for Engingeered Self-Organising Spatial Structures"
description = "Presentation @ACSOS 2024"
outputs = ["Reveal"]

+++

# An Aggregate Vascular Morphogenesis Controller for Engingeered Self-Organising Spatial Structures

[Angela Cortecchia](mailto:angela.cortecchia@unibo.it) <!--<i class="fa-solid fa-computer"></i>-->,
[Danilo Pianini](mailto:danilo.pianini@unibo.it) <!--<i class="fa-solid fa-computer"></i>-->,
[Giovanni Ciatto](mailto:giovanni.ciatto@unibo.it) <!--<i class="fa-solid fa-computer"></i>-->,
and
[Roberto Casadei](mailto:roby.casadei@unibo.it) <!--<i class="fa-solid fa-computer"></i>-->



<div style="text-align: center; width: 100%;">
<img src="example-background.svg" style="width: 40%" />

<!-- <i class="fa-solid fa-computer"></i> Department of Computer Science and Engineering, University of Bologna, Cesena (FC), Italy -->
</div>

---

{{< multicol>}}

{{< col >}}
{{% fragment %}}
### Plants
![plant image](images/plant-svgrepo-com.svg)
{{%/ fragment %}}
{{</ col >}}

{{< col >}}
{{% fragment %}}
### Organizations
![organization order image](images/organization-order-svgrepo-com.svg)
{{%/ fragment %}}
{{</ col >}}

{{< col >}}
{{% fragment %}}
### Flocking swarms
![organization order image](images/flock.svg)
{{%/ fragment %}}
{{</ col >}}

{{</ multicol >}}

{{% fragment %}}
# What do they have in common?
{{%/ fragment %}}

{{< frag c="## A runtime generated hierarchical structure" >}}

---

# The Vascular Morphogenesis Controller

{{< multicol >}}

{{< col class="col-8">}}
<p class = "fragment" data-fragment-index="0">The <b>VMC</b> is a model for the growth of artificial structures over time.</p>
<p class = "fragment" data-fragment-index="1">It models tree-like structures, in which every node can get information from the environment.</p>
<p class = "fragment" data-fragment-index="2">The leaves of the tree start by sending the amount of <b>success</b> they sense to the root.</p>
<p class = "fragment" data-fragment-index="3">The root then sends back an amount of <b>resources</b> based on the success received from the leaves, regulating the tickness of their connections.</p>
<h3 class = "fragment" data-fragment-index="4"><i class="fa-solid fa-arrow-right"></i> But it has some limitations</h3>
<p class = "fragment" data-fragment-index="5"><i class="fa-solid fa-triangle-exclamation"></i> VMC assumes that organizations have <b>only</b> a tree structure.</p>
<p class = "fragment" data-fragment-index="6"><i class="fa-solid fa-triangle-exclamation"></i>VMC assumes strict <b>synchronous operations</b>.</p>
<p class = "fragment" data-fragment-index="7"><i class="fa-solid fa-angles-right"></i>Restricting the model usefulness, leading to <b>abstraction gaps</b>.</p>
{{</ col >}}

{{< col >}}
<div class="r-stack">
  <img
    class="fragment current-visible"
    data-fragment-index="0"
    src="./images/tree.pdf"
    width="600"
    height="500"
  />
  <img
    class="fragment current-visible"
    data-fragment-index="1"
    src="./images/treeWithSensing.pdf"
    width="600"
    height="500"
  />
  <img
    class="fragment current-visible"
    data-fragment-index="2"
    src="./images/treeWithSucc.pdf"
    width="600"
    height="500"
  />
  <img
    class="fragment current-visible"
    data-fragment-index="3"
    src="./images/treeWithRes.pdf"
    width="600"
    height="500"
  />
  <img
    class="fragment"
    data-fragment-index="4,5,6,7"
    src="./images/treeWithResourcesandSuccess.pdf"
    width="600"
    height="500"
  />
</div>
{{</ col >}}
{{</ multicol >}}

---

# Possible Solution?

An implementation as a **Field-based** computation with the **Aggregate Computing** paradigm!

---

# What is Aggregate Computing?

<img src="./images/acDevices.pdf" width=70%>

A macro-programming approach that defines the **collective behavior** of heterogeneous devices in a **self-organizing system**.

Based on Field Calculus abstractions, it operates in terms of *field*: a distributed data structure.

--- 

# The **Aggregate** Vascular Morphogenesis Controller

## Model

---

# The **Aggregate** Vascular Morphogenesis Controller

## Implementation

(roots, regions, flaws)
open source, soon in standard lib -> pattern organizzativi che prima non c'erano
validation made by qualitative approach

---

# The **Aggregate** Vascular Morphogenesis Controller

## distinctive features 
(multiple leaders, growth and shrink, merge and split)

---

# Experiments

gif varie con fragment

---

# Conclusions / future works 

per cosa possiamo usarlo?
