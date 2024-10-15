Challenge Setup
================

Install the challenge,

```bash
task labs:jurassic-net:setup
```

> [!IMPORTANT]
>  Takes about 70 seconds from deployment to healthy state.

Jurassic Net
=========================================================

In a world where dinosaurs rule the tech landscape, Certosaurus is the self-proclaimed "security specialist" of *Jurassic Net*, the dino version of the internet. Certosaurus oversees the security of the network, ensuring everything is running smoothly—or so he claims.

Meet the Jurassic Net Team
==========================

1. **Certosaurus (Security Specialist):**  
   Certosaurus is responsible for safeguarding connections across the network. He takes his job seriously, but he has a habit of being… a little forgetful. Certosaurus likes to say, “Back in my day, we didn’t need all these complicated protocols!”

2. **DNS-raptor (The Swift Router):**  
   DNS-raptor is the fastest router in all of Jurassic Net, directing data traffic with lightning speed. He depends on Certosaurus to keep the network secure. When things go awry, DNS-raptor ends up in a frenzy, scrambling to reroute everything.

A Typical Day on Jurassic Net
==============================

Certosaurus is lounging under a tree, enjoying the shade, when DNS-raptor zips over, feathers ruffled and in a hurry.  
“Certosaurus! The network’s down, and everything’s out of whack!” DNS-raptor hisses.

Certosaurus blinks and stretches, unbothered. “Calm down, DNS-raptor. It’s probably just a minor glitch. Back in my day, we didn’t have these fancy systems anyway.”

“But everyone’s locked out of the secure servers! What happened?” DNS-raptor demands.

Certosaurus scratches his chin thoughtfully. “Could be anything—a bit of dust, some cosmic rays, who knows? Let’s have a look.” He meanders over to his control panel, examining the logs with a lazy eye.

DNS-raptor, clearly anxious, paces in circles. “Can you hurry up? The herbivores are starting to panic without access to DinoTube!”

Certosaurus finally presses a button, and with a beep, the network comes back online. “There you go! Probably just a little prehistoric hiccup.”

DNS-raptor sighs in relief, rushing off to restore the connections. Certosaurus watches him go, chuckling to himself. “These young dinos and their panic—what a time to be extinct!”  

And just like that, Jurassic Net is safe again… until Certosaurus’s forgetfulness stirs up trouble once more...


Finding Certosaurus
=================

You will find him in the `museum-jurassic-net` namespace in the downstream cluster. Go to the [button label="SUSE Observability" style="primary"](tab-3), and then follow these steps:

1. Expand the hamburger menu in the top left corner and click on `Services`.
2. In the top-right corner, filter to your cluster (`[[ Instruqt-Var key="DOWNSTREAM_CLUSTER_NAME" hostname="management" ]]`) and the `museum-jurassic-net` namespace.

3. Click on the `topology` perspective to see how Certosaurus is performing.


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
task labs:jurassic-net:resolve
```


Challenge Teardown
==================

```bash
task labs:jurassic-net:teardown
```