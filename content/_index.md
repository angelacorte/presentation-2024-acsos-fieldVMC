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

{{< multicol >}}

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

{{< frag c="## They all have a runtime generated hierarchical structure" >}}

---

# The Vascular Morphogenesis Controller

{{< multicol >}}

{{< col >}}
<p class = "fragment" data-fragment-index="0">The <b>VMC</b> is a model for the growth of artificial structures over time.</p>
<p class = "fragment" data-fragment-index="1">It models tree-like structures, in which every node can get information from the environment.</p>
<p class = "fragment" data-fragment-index="2">The leaves of the tree start by sending the amount of <b>success</b> they sense to the root.</p>
<p class = "fragment" data-fragment-index="3">The root then sends back an amount of <b>resources</b> based on the success received from the leaves, regulating the tickness of their connections.</p>
<h3 class = "fragment" data-fragment-index="4">But it has some limitations</h3>
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
<p class = "fragment" data-fragment-index="5">VMC assumes that organizations have <b>only</b> a tree structure.</p>
</div>

{{</ col >}}

{{</ multicol >}}




<!-- <div class="r-stack">
  <img
    class="fragment fade-out"
    data-fragment-index="0"
    src="https://picsum.photos/450/300"
    width="450"
    height="300"
  />
  <img
    class="fragment current-visible"
    data-fragment-index="0"
    src="https://picsum.photos/300/450"
    width="300"
    height="450"
  />
  <img
    class="fragment"
    src="https://picsum.photos/400/400"
    width="400"
    height="400"
  />
</div> -->
<!-- what it is -->
<!-- limitations -->
<!-- how we want to address them -->

---

# What is Aggregate Computing?

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
