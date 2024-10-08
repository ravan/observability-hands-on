Challenge Setup
================

Install the challenge,

```bash
task labs:dino-diner:setup
```

> [!IMPORTANT]
>  Takes about 70 seconds from deployment to healthy state.

Welcome to Dinosaur Diner: The World's Oldest Restaurant!
=========================================================

In a bustling corner of the prehistoric world lies Dinosaur Diner, the go-to spot for hungry dinos of all shapes and sizes. Here, five prehistoric culinary microservices keep the food and fun flowing—until one dinosaur chef gets a bit too... slow.


### Meet the Dino Diner Team

1. **Bronto Burger (The Head Chef):**  
   Bronto is a giant, slow-moving but reliable chef who takes his time to whip up delicious dino-sized burgers for the carnivores and plant-based dishes for the herbivores. Every meal depends on Bronto, and he has to make sure the T-Rex isn’t too close before serving—nobody wants their lunch interrupted by a dino stampede!

2. **T-Rex Tracker (The Hungry Guardian):**  
   T-Rex Tracker ensures that the dangerous T-Rex stays at a safe distance from the Diner. It constantly tracks the T-Rex's whereabouts, ensuring Bronto knows when it’s safe to serve and when it’s time to close up shop. However, if T-Rex Tracker misses a beat, the kitchen might go into panic mode!

3. **Herbivore Hideout (The Salad Expert):**  
   This service ensures that the herbivores, like the gentle Stegosaurus and Diplodocus, get their fresh leafy greens on time. But *Herbivore Hideout* can only prepare the salad bar once it gets word from *PteroPost* that it’s safe. When the salads are late, the herbivores get cranky, and trust me, no one wants an upset Diplodocus.

4. **PteroPost (The Gossiping Messenger):**  
   PteroPost is the Diner’s speedy communication system, flying between services and delivering updates. It sends the latest orders from Bronto Burger to the rest of the kitchen crew and coordinates with *Triceratops Transport* to make sure everyone’s in the right place. Without *PteroPost*, the kitchen would be a disaster, and the orders would never make it to the tables.

5. **Triceratops Transport (The Sluggish Waiter):**  
   This once-speedy waiter is now the bane of *Dinosaur Diner*’s existence. Due to some recent memory stress and CPU overload (maybe from carrying too many trays?), *Triceratops Transport* is slowing everything down. Orders that used to be lightning fast are now delayed, and when Triceratops falls behind, the whole restaurant feels the pinch. Guests are left waiting at their tables, getting hungrier—and grumpier—by the minute.

---

## A Typical Day at the Diner (Gone Wrong)


It's a bustling afternoon at *Dinosaur Diner*. The line of hungry dinosaurs stretches all the way to the volcano, and the pressure's on!

**Bronto Burger** starts up the grill, preparing a fresh batch of Bronto-sized burgers for the carnivores. But before flipping the patties, Bronto checks in with the **T-Rex Tracker**: "Is it safe? Where’s the T-Rex?"  
*T-Rex Tracker* sends a reassuring message—“All clear! T-Rex is on the other side of the jungle.” Bronto gets to work.

Meanwhile, in the salad section, **Herbivore Hideout** is getting ready for a steady flow of leaf-eaters. But wait! Before chopping up some ferns, they need a status update from **PteroPost**. They can’t start serving until *PteroPost* delivers the "safe to graze" message. *PteroPost*, being the chatty bird it is, flaps around sending messages to everyone.

But just when things seem to be running smoothly, the orders hit a roadblock—**Triceratops Transport** has fallen behind again! As the restaurant’s only waiter, *Triceratops* has developed a terrible habit of getting stuck halfway between the kitchen and the tables. Poor *Triceratops Transport* can barely carry a single order without collapsing in a heap.

**Bronto Burger** yells from the grill: “Where are the burgers going?!”  
**Herbivore Hideout** grumbles: “These salads are wilting!”  
**PteroPost** swoops down to investigate and sends a message: “Orders are delayed. Triceratops is taking another nap.”

Will the team pull together in time to serve the perfect dino-sized meal? Or will *Triceratops Transport* finally crash under the pressure? Only observability can save *Dinosaur Diner* from extinction!



Lets start observing the diner?
===============================


```bash
task labs:dino-diner:trigger
```

> [!IMPORTANT]
>  Takes about 3 minutes from deployment to unhealthy state.

> [!NOTE]
> Learning platform instructions,
> Suse Observability steps


Finding the diner
=================

The diner is running in the `museum-dino-diner` namespace in the downstream cluster. Go to the [button label="SUSE Observability" style="primary"](tab-3), and then follow these steps:

1. Expand the hamburger menu in the top left corner and click on `Services`.
2. In the top-right corner, filter to your cluster (`[[ Instruqt-Var key="DOWNSTREAM_CLUSTER_NAME" hostname="management" ]]`) and the `museum-dino-diner` namespace.

3. Click on the `topology` page to see how the diner is performing.


First steps in troubleshooting
==============================

> [!NOTE]
> Learning platform instructions,
> Suse Observability steps


Diagnosis
=========

> [!NOTE]
> Learning platform instructions,
> Suse Observability steps


Fixing the issue
================

> [!NOTE]
> Learning platform instructions,
> Suse Observability steps

```bash
task labs:dino-diner:resolve
```


Challenge Teardown
==================

```bash
task labs:dino-diner:teardown
```