# Fitness Machine Service

[Home Assistant](https://www.home-assistant.io/) [HACS](https://hacs.xyz/) custom component for working with fitness equipment with a Bluetooth interface.

The component is based on the [pyftms](https://github.com/dudanov/pyftms) library, which complies with the [Bluetooth Fitness Machine Service v1.0 standard](https://www.bluetooth.com/specifications/specs/fitness-machine-service-1-0/).

Component capabilities:

1. Automatically detect Bluetooth fitness devices nearby, notifying the user about it;
2. Setup Wizard, which allows you to easily configure the device by determining its type and set of sensors in automatic or manual modes. The set of sensors can be changed.
3. Collects training data from fitness equipment and allows you to set training parameters specific to the type of equipment.

Supported fitness machines:

1. **Treadmill**
2. **Cross Trainer** (Elliptical Trainer)
3. **Rower** (Rowing Machine)
4. **Indoor Bike** (Spin Bike)

Device view example for `FitShow FS-BT-D2 Indoor bike` fitness machine:

![image](images/main.png)

## Installation

### HACS

Follow [this guide](https://hacs.xyz/docs/faq/custom_repositories/) to add this git repository as a custom HACS repository. Then install from HACS as normal.

### Manual Installation

Copy `custom_components/ftms` into your Home Assistant `$HA_HOME/config` directory, then restart Home Assistant.
