+++

title = "An Aggregate Vascular Morphogenesis Controller for Engingeered Self-Organising Spatial Structures"
description = "Presentation @ACSOS 2024"
outputs = ["Reveal"]

+++

# An Aggregate Vascular Morphogenesis Controller for Engingeered Self-Organising Spatial Structures

[**Angela Cortecchia**](mailto:angela.cortecchia@unibo.it) <!--<i class="fa-solid fa-computer"></i>-->,
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

{{< frag c="## A runtime-generated hierarchical structure" >}}

---

# The Vascular Morphogenesis Controller

{{< multicol >}}

{{< col class="col-8">}}
<p class = "fragment" data-fragment-index="0">The <b>VMC</b> is a model for the growth of artificial structures over time.</p>
<p class = "fragment" data-fragment-index="1">It models tree-like structures, in which every node can <b>get information from the environment</b>.</p>
<p class = "fragment" data-fragment-index="2">The leaves of the tree start by sending the amount of <b>success</b> they sense to the root.</p>
<p class = "fragment" data-fragment-index="3">The root then sends back an amount of <b>resources</b> based on the success received from the leaves, regulating the tickness of their connections.</p>
<h3 class = "fragment" data-fragment-index="4"><i class="fa-solid fa-arrow-right"></i> But it has some limitations</h3>
<p class = "fragment" data-fragment-index="5"><i class="fa-solid fa-triangle-exclamation"></i>VMC assumes strict <b>synchronous operations</b>.</p>
<p class = "fragment" data-fragment-index="11"><i class="fa-solid fa-triangle-exclamation"></i> VMC assumes that organizations have <b>only</b> a tree structure.</p>
<p class = "fragment" data-fragment-index="12"><i class="fa-solid fa-angles-right"></i>Could restricts the model usefulness, leading to <b>abstraction gaps</b>.</p>
{{</ col >}}

{{< col >}}
<div class="r-stack">
  <img
    class="fragment current-visible"
    data-fragment-index="0"
    src="images/tree.svg"
    width="180%"
    height="170%"
  />
  <img
    class="fragment current-visible"
    data-fragment-index="1"
    src="images/treeWithSensing.svg"
    width="180%"
    height="170%"
  />
  <img
    class="fragment current-visible"
    data-fragment-index="2"
    src="images/treeWithSuccess.svg"
    width="180%"
    height="170%"
  />
  <img
    class="fragment current-visible"
    data-fragment-index="3"
    src="images/treeWithResources.svg"
    width="180%"
    height="170%"
  />
  <img
    class="fragment current-visible"
    data-fragment-index="4"
    src="images/treeWithResourcesandSuccess.svg"
    width="180%"
    height="170%"
  />
  <img
      class="fragment current-visible"
      data-fragment-index="5"
      src="images/firstStep.svg"
      width="180%"
      height="170%"
    />
  <img
      class="fragment current-visible"
      data-fragment-index="6"
      src="images/secondStep.svg"
      width="180%"
      height="170%"
    />
  <img
      class="fragment current-visible"
      data-fragment-index="7"
      src="images/thirdStep.svg"
      width="180%"
      height="170%"
    />
  <img
      class="fragment current-visible"
      data-fragment-index="8"
      src="images/fourthStep.svg"
      width="180%"
      height="170%"
    />
  <img
      class="fragment current-visible"
      data-fragment-index="9"
      src="images/fifthStep.svg"
      width="180%"
      height="170%"
    />
  <img
      class="fragment current-visible"
      data-fragment-index="10"
      src="images/sixthStep.svg"
      width="180%"
      height="170%"
    />
  <img
    class="fragment current-visible"
    data-fragment-index="11"
    src="images/graph.svg"
    width="180%"
    height="170%"
  />
  <img
    class="fragment current-visible"
    data-fragment-index="12"
    src="images/graph.svg"
    width="180%"
    height="170%"
  />
</div>
{{</ col >}}
{{</ multicol >}}

---

# A Possible Solution?

An implementation as a **Field-based** computation with the **Aggregate Computing** paradigm!

---

# What is Aggregate Computing?

<img src="./images/acDevices.svg" width=70%>

A macro-programming approach that defines the **collective behavior** of heterogeneous devices in a **self-organizing system**.

Based on Field Calculus abstractions, it operates in terms of *field*: a distributed data structure.

--- 

# The **Aggregate** Vascular Morphogenesis Controller

## Model

{{< multicol >}}

{{< col class="col-8">}}
<p class = "fragment" data-fragment-index="0">A node represents an <b>agent</b>.</p>
<p class = "fragment" data-fragment-index="1">A neighboring link denotes the possibility of two agents to <b>communicate</b>.</p>
<p class = "fragment" data-fragment-index="2">Each agent is assumed to have <b>sensors</b>:</br><em>success, resource, position and distance.</em></p>
<p class = "fragment" data-fragment-index="3">And <b>actuators</b>:</br><em>spawning and destroying.</em></p>

{{</ col >}}

{{< col >}}
<div class="r-stack">
  <img
    class="fragment current-visible"
    data-fragment-index="0"
    src="images/agent.svg"
    width="100%"
    height="100%"
  />
  <img
    class="fragment current-visible"
    data-fragment-index="1"
    src="images/connection.svg"
    width="180%"
    height="170%"
  />
  <img
    class="fragment current-visible"
    data-fragment-index="2"
    src="images/sensors.svg"
    width="180%"
    height="170%"
  />
  <img
    class="fragment current-visible"
    data-fragment-index="3"
    src="images/actuators.svg"
    width="180%"
    height="170%"
  />
</div>
{{</ col >}}
{{</ multicol >}}

---

# The **Aggregate** Vascular Morphogenesis Controller

## Implementation

{{< multicol >}}

{{% col class="text-start col-md-7" %}}

Structures as <b>graphs</b> are supported. 

To define the forward and backward flows of resources and success, we used the _self-organizing coordination regions_ pattern, hence supporting <b>multiple trees</b> and a <b>dynamic</b>, <b>resilient set of trees</b>.

<p class = "fragment" data-fragment-index="0">Given a network of devices, the <b>SCR</b> pattern performs simultaneously four steps:</p>
<ol>
  <li class="fragment" data-fragment-index="1">Elects sparse <b>leaders</b> among candidates;</li>
  <li class="fragment" data-fragment-index="3">Evolves <b>regions</b> from leaders;</li>
  <li class="fragment" data-fragment-index="4">Creates <b>upstream</b> information <b>flows</b> towards the leader;</li>
  <li class="fragment" data-fragment-index="5">Performs <b>decision-making</b> at the leader and <b>downstream decisions</b>.</li>
</ol>

{{%/ col %}}

{{% col %}}
<div class="r-stack">
  <img
    class=" current-visible"
    src="images/network-1.svg"
    width="100%"
    height="100%"
  />
  <img
    class="fragment current-visible"
    data-fragment-index="1"
    src="images/network-candidates.svg"
    width="180%"
    height="170%"
  />
  <img
    class="fragment current-visible"
    data-fragment-index="2"
    src="images/network-leaders.svg"
    width="180%"
    height="170%"
  />
  <img
    class="fragment current-visible"
    data-fragment-index="3"
    src="images/network-regions.svg"
    width="180%"
    height="170%"
  />
    <img
    class="fragment current-visible"
    data-fragment-index="4"
    src="images/network-upstream.svg"
    width="180%"
    height="170%"
  />
    <img
    class="fragment current-visible"
    data-fragment-index="5"
    src="images/network-downstream2.svg"
    width="180%"
    height="170%"
  />
</div>
{{%/ col %}}

{{</ multicol >}}


<!-- SCR addresses problem decomposition and task assignment in distributed settings by: (i) electing sparse lead- ers; (ii) evolving regions from leaders; (iii) creating upstream information flows [14] towards the leader; (iv) performing decision-making at the leader and downstreaming decisions. -->


<!-- (roots, regions, flaws) -->
<!-- open source, soon in standard lib -> pattern organizzativi che prima non c'erano -->
<!-- validation made by qualitative approach -->

---

# The **Aggregate** Vascular Morphogenesis Controller

## distinctive features 
(multiple leaders, growth and shrink, merge and split)

--- 

# Self-Construction

{{< multicol >}}
{{< col >}}
<img src="images/oneRootWithIndex.gif" alt="One root sequence">
{{</ col >}}

{{% col %}}
Some text here
{{%/ col %}}

{{</ multicol >}}

---

# Self-Repairing

{{< multicol >}}
{{< col >}}
<img src="images/cuttingWithIndex.gif" alt="One root sequence">
{{</ col >}}

{{% col %}}
Some text here
{{%/ col %}}

{{</ multicol >}}

---

# Self-Integration

{{< multicol >}}
{{< col >}}
<img src="images/graftWithIndex.gif" alt="One root sequence">
{{</ col >}}

{{% col %}}
Some text here
{{%/ col %}}

{{</ multicol >}}

---

# Self-Optimization

{{< multicol >}}
{{< col >}}
<img src="images/graftWithSpawningWithIndex.gif" alt="One root sequence">
{{</ col >}}

{{% col %}}
fixa la gif che ha le immagini sbagliate
{{%/ col %}}

{{</ multicol >}}

---

# Self-Segmentation

{{< multicol >}}
{{< col >}}
<img src="images/graftWithMoreLeadersWithIndex.gif" alt="One root sequence">
{{</ col >}}

{{% col %}}
Some text here
{{%/ col %}}

{{</ multicol >}}

---

# Conclusions / future works 

per cosa possiamo usarlo?
