Challenge Setup
================

Install the challenge,

```bash
task labs:forgetasaurus:setup
```

> [!Timing]
>  Takes about 70 seconds from deployment to healthy state.

The Memory-Eating Dinosaur
==========================================

Forgetasaurus represents the elusive, mythical creature that causes memory leaks and out-of-memory (OOM) errors in your microservice ecosystem. Every time your services struggle to handle memory, it's because the Forgetasaurus is slowly "eating" the memory away, leading to inevitable crashes.

## Dinosaurs that play in this park
- **TyrannoDB** – "TyrannoDBrex: Unaffected by Forgetasaurus"  
  TyrannoDB is too big and strong to be impacted by Forgetasaurus. It keeps hoarding data without issue.
  
- **Raptoring Service** – "VelociFetcher: Forgetasaurus’s Favorite Snack"  
  VelociFetcher is constantly hit by Forgetasaurus. As it tries to respond to Brontoclient’s demands, Forgetasaurus quietly drains its memory, causing eventual OOM failures.

- **Brontoclient** – "Brontoclient: Oblivious to Forgetasaurus"  
  Brontoclient doesn't even realize that Forgetasaurus exists. It just keeps asking for more data, unaware that VelociFetcher is being silently attacked by this memory-hungry dino.


Letting Forgetasaurus Loose
===========================

_"Forgetasaurus: Your memory’s worst nightmare!"_


```bash
task labs:forgetasaurus:trigger
```

> [!Timing]
>  Takes about 3 minutes from deployment to unhealthy state.

> [!TODO]
> Learning platform instructions
> Suse Observability steps


Finding the Forgetasaurus
========================

The Forgetasaurus is running in the `museum-forgetasaurus` namespace in the downstream cluster. Go to the [button label="SUSE Observability" style="primary"](tab-3), and then follow these steps:

1. Expand the hamburger menu in the top left corner and click on `Pods`.
2. In the top-right corner, filter to your cluster (`[[ Instruqt-Var key="DOWNSTREAM_CLUSTER_NAME" hostname="management" ]]`) and the `museum-forgetasaurus` namespace.

3. Click on the `raptoring-service` pod to see its details.


First steps in troubleshooting
==============================

> [!TODO]
> Learning platform instructions
> Suse Observability steps


Diagnosis
=========

> [!TODO]
> Learning platform instructions
> Suse Observability steps


Fixing the issue
================

> [!TODO]
> Learning platform instructions
> Suse Observability steps

```bash
task labs:forgetasaurus:resolve
```


Challenge Teardown
==================

```bash
task labs:forgetasaurus:teardown
```