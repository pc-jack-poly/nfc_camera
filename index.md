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
<p>Mobile payment today is dominated by two technologies: NFC and optical barcodes. NFC offers superior security, usability, and accessibility, but nearly half of smartphones either lack NFC hardware or have it disabled. This gap forces many users to resort to barcode-based payments, despite their weaker security and user experience. In this work, we present MagCode+, a physical side-channel communication mechanism that allows an NFC reader to transmit data directly to a smartphone camera by producing standards-compliant barcodes through benign magnetic interference on the CMOS sensor. Unlike prior approaches that emulate barcode content, MagCode+ introduces a barcode-native modulation and decoding pipeline that generates barcodes identical to those expected by commercial scanners, enabling seamless interoperability with existing payment and retail infrastructures. We prototype both the NFC-side waveform engine and smartphone-side decoding pipeline and evaluate the system across 11 devices. MagCode+ natively supports six major 1D barcode standards, achieves up to 537bps throughput, and delivers widely used payment barcodes such as CODE128 within 0.28s. These results demonstrate that MagCode+ forms an immediately deployable bridge between NFC infrastructure and non-NFC smartphones while requiring no modifications to existing barcode-based ecosystems.</p>
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
