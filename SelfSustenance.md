# Self-sustaining pinephone

As a "minimalist" the goal is to feel free in spirit. This requires pure open standards to know that your digital belongings can migrate with you in the future as well as being able to do what you need with few gadgets.

What is needed to ensure that no other HW than one pinephone is ever needed simultaneously? This is my idea how to set that up. Now I need to learn more about the possibilities of achieving this.

- A Basic (Minimal?) Linux (BML) setup on a bootable sdcard.
The BML shall have scripts prepared to easily install itself on emmc if desired.
  - The BML shall support LTE and a basic browser in order to download new images that can be 'flashed' onto new SDcards.
  - The BML shall preferrably support USB-OTG sdcard adapter to avoid constant back cover removal.
    - This means working OTG support, requiring the HW patch on my Pinephone 1.2
- Android apps need to be runnable to manage every day life encounters with society such as software based 2FA.
  - Preferrably via anbox, but using GloDroid (https://github.com/GloDroid/glodroid_manifest/releases) as a separate sdcard to boot is the current target.
  - GloDroid currently installs using a fairly long series of fastboot operations. This process need to get an alternative as a clean sdcard flashable image with all android partitions needed.
  - Maybe additional TWRP-like features are needed in GloDroid to cheat SafetyNet if needed. Maybe microG is enough (https://github.com/GloDroid/glodroid_manifest/issues/19)
