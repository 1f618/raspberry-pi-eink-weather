# Ansible Raspberry Pi E Ink Weather 🐂 🖋️ 🥧 ⛈️

This is an Ansible port of the excellent [Raspberry Pi E-Ink Weather Station using Python](https://learn.adafruit.com/raspberry-pi-e-ink-weather-station-using-python) demo, originally created by [Melissa LeBlanc-Williams](https://learn.adafruit.com/u/MakerMelissa) for [Adafruit Industries](https://www.adafruit.com).

Instead of running through the steps of the demo manually, this Ansible playbook **handles the entire installation automatically**. 🪄 ✨

Included in this port is an Ansible role, `1f618.circuitpython_on_linux`, which installs CircuitPython on a Raspberry Pi.

## Prerequisites

* A Raspberry Pi, running **Raspberry Pi OS Lite** (or full-fledged Raspberry Pi OS), with SSH access already configured and a [Monochrome E-Ink Bonnet](https://www.adafruit.com/product/4687) attached
* Ansible
* Installation of the required Ansible Galaxy role(s)
  ```
  ansible-galaxy install -r requirements.yml
  ```

## Usage

* Update `hosts.yml` with the connection details for your Pi
* Update the `open_weather_token` and `location` vars in `main.yml`
* Run the playbook:

```
ansible-playbook main.yml
```

## Special Thanks

* [Melissa LeBlanc-Williams](https://learn.adafruit.com/u/MakerMelissa) for writing the [original guide](https://learn.adafruit.com/raspberry-pi-e-ink-weather-station-using-python)
* [Jeff Geerling](https://www.jeffgeerling.com) for [geerlingguy.pip](https://galaxy.ansible.com/geerlingguy/pip),  the inspiring [Ansible for DevOps book](https://www.ansiblefordevops.com), and the companion [Ansible 101 YouTube series](https://www.youtube.com/watch?v=goclfp6a2IQ&list=PL2_OBreMn7FqZkvMYt6ATmgC0KAGGJNAN)
* Everyone at Adafruit for their work on [CircuitPython](https://circuitpython.org) and the [Monochrome E-Ink Bonnet](https://www.adafruit.com/product/4687)
