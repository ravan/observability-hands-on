Challenge Setup
================

Install the challenge,

```bash
task labs:certosaurus:setup
```

> [!IMPORTANT]
>  Takes about 70 seconds from deployment to healthy state.

Certosaurus
=========================================================

Certosaurus is the trusted gatekeeper of security. This old dino’s job is to make sure all the connections between services are secure and properly certified. With a collection of certificates as long as its tail, Certosaurus is known for its meticulous (though sometimes outdated) ways.

Today his outdated ways is causing all sorts of chaos for him and he just can't get started.

Figure out what is causing this.



Finding Certosaurus
=================

You will find him in the `museum` namespace in the downstream cluster. Go to the [button label="SUSE Observability" style="primary"](tab-3), and then follow these steps:

1. Expand the hamburger menu in the top left corner and click on `Services`.
2. In the top-right corner, filter to your cluster (`[[ Instruqt-Var key="DOWNSTREAM_CLUSTER_NAME" hostname="management" ]]`) and the `museum` namespace.

3. Click on the `pod` to see how Certosaurus is performing.


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
task labs:certosaurus:resolve
```


Challenge Teardown
==================

```bash
task labs:certosaurus:teardown
```