---
layout: default
title: ""
---

## Abstract

<div class="abstract">
{% assign _png = site.static_files | where: "path", "/assets/images/scenario.png" | first %}
<div class="figure-right">
  {% if _png %}
    <img src="{{ 'assets/images/scenario.png' | relative_url }}" alt="Attack scenarios figure" />
  {% else %}
    <iframe class="pdf-frame" src="{{ 'assets/images/scenario.pdf' | relative_url }}#toolbar=0&navpanes=0&scrollbar=0"></iframe>
  {% endif %}
  <div class="caption">MagCode+ Application Scenarios</div>
</div>
<p>Recent works demonstrated that speech recognition systems or voice assistants can be manipulated by malicious voice commands, which are injected through various inaudible media, such as ultrasound, laser, and electromagnetic interference (EMI). In this work, we explore a new kind of inaudible voice attack through the magnetic interference induced by a wireless charger.  Essentially, we show that the microphone components of smart devices suffer from severe magnetic interference when they are enjoying wireless charging, due to the absence of effective protection against the EMI at low frequencies (100 kHz or below). By taking advantage of this vulnerability, we have developed an inaudible voice attack termed ParasiteAttack, designed to inject malicious voice commands into smart devices during wireless charging. This attack utilizes an accessory equipment known as a parasite label to replicate the victim's voiceprint first and then deliver inaudible voice commands. We conducted comprehensive experiments involving 17 victim devices (including iPhones, Huawei, Samsung, etc.) and 6 types of voice assistants (such as Siri, Google STT, Bixby, etc.). The evaluation results demonstrate the feasibility of the proposed attack under commercial wireless charging conditions. To address this emerging threat, we present a privacy-preserving on-device defense framework that leverages small language models (SLMs) to detect abnormal magnetic voice commands. The framework is evaluated across five representative SLMs (e.g., SpeechLLM, Aero-1-Audio, etc.), achieving an average detection accuracy of 96.9% and an equal error rate of 3.06%, while maintaining an average real-time inference latency below 500 ms on mobile devices. These results confirm that the proposed approach provides an effective and responsive on-device defense against magnetic voice command attacks.</p>
</div>

<!-- ## Teaser Video
<iframe width="560" height="315" src="https://www.youtube.com/embed/-JItdyhV1ik" title="IEEE S&amp;P 2023 Teaser Video &quot;Inducing Wireless Chargers to Voice Out for Inaudible Command Attacks&quot;" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe> -->

## Compatibility: Universal Support for Commercial Barcode Standards

Our approach is compatible with nearly all existing commercial barcode standards, ensuring broad applicability across diverse retail and industrial environments.

<div class="barcode-gallery">
  <div class="barcode-item">
    <img src="{{ 'assets/images/EAN8.png' | relative_url }}" alt="EAN-8 Barcode">
    <div class="barcode-label">EAN-8</div>
  </div>
  <div class="barcode-item">
    <img src="{{ 'assets/images/EAN13.png' | relative_url }}" alt="EAN-13 Barcode">
    <div class="barcode-label">EAN-13</div>
  </div>
  <div class="barcode-item">
    <img src="{{ 'assets/images/UPC-A.png' | relative_url }}" alt="UPC-A Barcode">
    <div class="barcode-label">UPC-A</div>
  </div>
  <div class="barcode-item">
    <img src="{{ 'assets/images/UPCE.png' | relative_url }}" alt="UPC-E Barcode">
    <div class="barcode-label">UPC-E</div>
  </div>
  <div class="barcode-item">
    <img src="{{ 'assets/images/CODE39.png' | relative_url }}" alt="Code 39 Barcode">
    <div class="barcode-label">Code 39</div>
  </div>
  <div class="barcode-item">
    <img src="{{ 'assets/images/CODE128.png' | relative_url }}" alt="Code 128 Barcode">
    <div class="barcode-label">Code 128</div>
  </div>
</div>

## Demo: NFC-Enabled Communication via Commercial Barcodes
<div class="video-container-50-left">
  <video controls preload="metadata">
    <source src="{{ 'assets/videos/demo_recording.mp4' | relative_url }}" type="video/mp4">
    Your browser does not support the video tag.
    <a href="{{ 'assets/videos/demo_recording.mp4' | relative_url }}">Download video</a>
  </video>
  
</div>


<!-- ## Paper

  @inproceedings{dai2022inducing,  
    title={Inducing wireless chargers to voice out for inaudible command attacks},  
    author={Dai, Donghui and An, Zhenlin and Yang, Lei},  
    booktitle={2023 IEEE Symposium on Security and Privacy (SP)},  
    pages={503--520},  
    year={2022},  
    organization={IEEE Computer Society}  
  }   -->
