# Suse Observability 

To get the best results from an interactive workshop, the system should be responsive.
Here we fine tune out of the box (oob) monitors and thresholds to fit the workshop scenarios.


## Prerequisites

- Suse Observability CLI
    In the Suse Observability web user interface, choose the `CLI` menu option and follow the installation instructions.

## Setup

We will disable some of the oob monitors and upload our fine tuned monitors.

```bash
task disable-oob-monitors
task upload-custom-monitors
```

## Teardown

Once the workshop is complete, we can re-enable the oob monitors and remove the fine tuned monitors.

```bash
task disable-custom-monitors
task enable-oob-monitors
task delete-custom-monitors
```
