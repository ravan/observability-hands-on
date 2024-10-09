# Suse Observability 

To get the best results from an interactive workshop, the system should be responsive.
Here we fine tune out of the box (oob) monitors and thresholds to fit the workshop scenarios.

We will disable some of the oob monitors and upload our fine tuned monitors.
Once the workshop is complete, we can re-enable the oob monitors and remove the fine tuned monitors.

## Prerequisites

- Suse Observability CLI
    In the Suse Observability web user interface, choose the `CLI` menu option and follow the installation instructions.

## Commands

### Disable the oob monitors

```bash
task disable-oob-monitors
```

### Enable the oob monitors

```bash
task enable-oob-monitors
```