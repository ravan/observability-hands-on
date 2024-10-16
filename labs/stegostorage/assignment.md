Challenge Setup
================

Install the challenge,

```bash
task labs:stegostorage:setup
```

> [!IMPORTANT]
>  Takes about 70 seconds from deployment to healthy state.

Stego Storage Hits a Snag
=========================================================

In the prehistoric realm of Jurassic Net, data storage is managed by Stego Storage, the dinosaur known for keeping everyone’s precious files safe. Stego Storage is famous for its massive plates, perfect for holding vast amounts of data. But today, something strange has happened, and Stego Storage is at a loss.

As Stego Storage prepares to save files, a peculiar message flashes on the stone tablets: “Storage Unavailable.” Stego Storage scratches his head and checks his equipment. Everything looks fine… or does it?

He mutters to himself, “I’m sure I set everything up just right. But where did all the space go?”

The other dinosaurs start lining up, ready to save their files, but Stego Storage can’t seem to find the missing piece. He tries to retrace his steps, but something just isn’t adding up. The pressure’s on as he scrambles to figure out the mystery of the missing storage, while the other dinos grow impatient.

Will Stego Storage crack the code before the queue of angry dinosaurs gets out of control? Or is he destined to become the prehistoric scapegoat of the Jurassic Net?


Finding Stegostorage
=================

You will find him in the `museum` namespace in the downstream cluster. Go to the [button label="SUSE Observability" style="primary"](tab-3), and then follow these steps:

1. Expand the hamburger menu in the top left corner and click on `Services`.
2. In the top-right corner, filter to your cluster (`[[ Instruqt-Var key="DOWNSTREAM_CLUSTER_NAME" hostname="management" ]]`) and the `museum` namespace.

3. Click on the `topology` perspective to see how Stegostorage is performing.


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
task labs:stegostorage:resolve
```


Challenge Teardown
==================

```bash
task labs:stegostorage:teardown
```