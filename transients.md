---
layout: default
title: Transients!!!
permalink: /transients/
---

<section class="intro">
  <h2>Shadow Transients!</h2>
  <p>
    This is where I would put my transients, IF I HAD ANY!!!
  </p>
</section>

---
layout: post
title: "{{ page.transient_name | default: 'Unknown Transient' }}"
transient_name: SN2025abc
thumbnail: "/assets/images/transients/sn2025abc_thumb.jpg"
coords: "RA: 12:34:56.78, Dec: +12:34:56.7"
classification: "SN II"
discovery_mag: "18.9"
tns_link: "https://www.wis-tns.org/object/2025abc"
---

<img src="{{ page.thumbnail }}" alt="{{ page.transient_name }} thumbnail" class="post-thumbnail">

**Coordinates:** {{ page.coords }}  
**Class:** {{ page.classification }}  
**Current Magnitude:** {{ page.current_mag | default: page.discovery_mag }}  
**TNS:** [View on TNS]({{ page.tns_link }})

---

Your write-up here. Describe the discovery, context, and any follow-up observations.
