Challenge Setup
================

Install the challenge,

```bash
task labs:configosaurus:setup
```

> [!IMPORTANT]
>  Takes about 70 seconds from deployment to healthy state.

Configosaurus and the Stubborn Message
=========================================================

There’s a dinosaur named Configosaurus, who handles all the important announcements. Configosaurus gets its messages from a magical stone tablet (also known as a ConfigMap) and proudly delivers them to the entire dino community. Every dino relies on Configosaurus to keep them up-to-date with the latest happenings.

The Problem
============

One day, the dino council decides to update the message on the stone tablet. Configosaurus struts out, ready to make the announcement. But when he opens his mouth, he ends up reciting the old message instead! The dinos look confused, but Configosaurus doesn’t seem to notice and just keeps repeating the outdated message.

Later, when a dino points out that the message is wrong, Configosaurus scratches his head. “But I got the message straight from the stone tablet! It must be the latest update, right?”

As the day goes on, Configosaurus keeps repeating the old message, despite the tablet having the new message etched on it. The dinos are bewildered, and Configosaurus is starting to wonder if he’s missing something.

“Maybe it’s the order I did things?” he mutters. “But that can’t be it… right?”

Little does Configosaurus know, he missed a critical step. Now, he’s stuck repeating the outdated message, while the new one remains unheard. The dinos shake their heads, wondering when Configosaurus will finally catch on.

Will Configosaurus figure out why he keeps saying the wrong thing, or will the dinos forever be stuck in the past?


Finding Configosaurus
=================

You will find him in the `museum` namespace in the downstream cluster. Go to the [button label="SUSE Observability" style="primary"](tab-3), and then follow these steps:

1. Expand the hamburger menu in the top left corner and click on `Pods`.
2. In the top-right corner, filter to your cluster (`[[ Instruqt-Var key="DOWNSTREAM_CLUSTER_NAME" hostname="management" ]]`) and the `museum` namespace.

3. Click on the `configosaurus` pod.


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
task labs:configosaurus:resolve
```


Challenge Teardown
==================

```bash
task labs:configosaurus:teardown
```