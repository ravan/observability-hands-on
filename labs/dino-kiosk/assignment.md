Challenge Setup
================

Install the challenge,

```bash
task labs:dino-kiosk:setup
```

> [!IMPORTANT]
>  Takes about 80 seconds from deployment to healthy state.
>  Takes another 40 seconds for ebpf connections to be made for services

Welcome to Dinosaur Kiosk: The World's Oldest Restaurant!
=========================================================

![dinokiosk](./dinokiosk.png)

In a bustling corner of the prehistoric world lies Dinosaur Kiosk, the go-to spot for hungry dinos of all shapes and sizes. Here, five prehistoric culinary microservices keep the food and fun flowing—until one dinosaur chef gets a bit too... slow.


### The Dino Kiosk Services

#### AI Model Service

The **AI Model** service is a critical component within the **Prod Cluster** responsible for generating predictions and performing training operations for dinosaur designs. This service processes requests from other components, such as the **Build-a-Dino** service, to provide AI-driven insights. With endpoints for both prediction and training, the AI Model service is designed to handle substantial compute loads, supporting latency and error rate configurations to simulate real-world model behavior.

#### Build-a-Dino Service

The **Build-a-Dino** service resides in the **Kiosk Cluster** and acts as the central hub for designing and ordering custom dinosaur models. This service interacts with both the **AI Model** service, to generate AI-powered designs, and the **Printing Service**, to initiate the printing process for ordered dinosaurs. It is equipped with endpoints for initiating the design process and placing orders, making it the primary interface for transforming design requests into tangible print jobs.

#### Printing Service

The **Printing Service** operates in the **Kiosk Cluster** and is responsible for managing 3D print jobs for dinosaur models. After receiving orders from the **Build-a-Dino** service, it submits them to the **Printing Queue** for processing. This service simulates typical printing behaviors, including initiating and monitoring print jobs, and interacts with the Printing Queue to manage the flow of print requests. The Printing Service is essential for maintaining an organized pipeline of print tasks, ensuring a smooth transition from design to physical output.

#### Printing Queue Service

The **Printing Queue** service is a queuing mechanism in the **Kiosk Cluster** that organizes and manages print jobs submitted by the **Printing Service**. It ensures that requests are stored and processed in an orderly fashion, facilitating the efficient handoff to the **3D Printer** service. The queue enables asynchronous processing, handling a backlog of print jobs while maintaining system stability and availability.

#### 3D Printer Service

The **3D Printer** service in the **Kiosk Cluster** is tasked with the final stage of dinosaur model creation. It retrieves queued print jobs from the **Printing Queue** and executes them, producing physical dinosaur models based on the ordered designs. The service also includes maintenance functionality to ensure operational reliability. By processing print jobs in a real-time environment, the 3D Printer service completes the workflow from design to a tangible output.

#### Frontend Service

The **Frontend** service is the user-facing component in the **Kiosk Cluster** that allows customers to browse available dinosaur designs and place orders. Acting as an interface to the **Build-a-Dino** service, the Frontend service routes customer requests to initiate new designs or place orders for printing. It provides a seamless user experience, enabling direct interaction with the design and ordering process, which is powered by the backend services within the architecture.


---


Lets start observing the kiosk?
===============================


```bash
task labs:dino-kiosk:trigger
```

> [!IMPORTANT]
>  Takes about 3 minutes from deployment to unhealthy state with span, http 5xxx and http response time monitors firing.

> [!NOTE]
> Learning platform instructions,
> Suse Observability steps


Finding the kiosk
=================

The kiosk is running in the `museum-dino-kiosk` namespace in the downstream cluster. Go to the [button label="SUSE Observability" style="primary"](tab-3), and then follow these steps:

1. Expand the hamburger menu in the top left corner and click on `Services`.
2. In the top-right corner, filter to your cluster (`[[ Instruqt-Var key="DOWNSTREAM_CLUSTER_NAME" hostname="management" ]]`) and the `museum-dino-kiosk` namespace.

3. Click on the `topology` page to see how the kiosk is performing.


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
task labs:dino-kiosk:resolve
```


Challenge Teardown
==================

```bash
task labs:dino-kiosk:teardown
```