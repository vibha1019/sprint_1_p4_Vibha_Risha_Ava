---
layout: page
title: Baking
permalink: /baking/
---

### Baking Recipes

<div style="text-align: center; margin-top: 20px;">
    <img src="{{ site.baseurl }}/images/sweet_treats.png" style="max-width: 100%; border-radius: 15px; box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);">
</div>

<div style="text-align: center; margin-top: 20px;">
    <select id="baking-menu" style="padding: 10px; border-radius: 5px; border: 1px solid #ccc; background-color: #f8f8f8;" onchange="location = this.value;">
        <option value="">Select a dish</option>
        <option value="{{ site.baseurl }}/baking/choco_chip_cookies">Choco Chip Cookies</option>
        <option value="{{ site.baseurl }}/baking/vanilla_layer_cakes">Vanilla Layer Cake</option>
        <option value="{{ site.baseurl }}/baking/sugar_cookies">Sugar Cookies</option>
        <option value="{{ site.baseurl }}/baking/lava_cakes">Lava Cake</option>
        <option value="{{ site.baseurl }}/baking/vanilla_cupcakes">Vanilla Cupcakes</option>
        <option value="{{ site.baseurl }}/baking/eclairs">Eclairs</option>
        <option value="javascript:randomPage()">Wildcard</option>
    </select>
</div>

<script>
    function randomPage() {
        var pages = [
            "{{ site.baseurl }}/baking/choco_chip_cookies",
            "{{ site.baseurl }}/baking/vanilla_layer_cakes",
            "{{ site.baseurl }}/baking/sugar_cookies",
            "{{ site.baseurl }}/baking/lava_cakes",
            "{{ site.baseurl }}/baking/vanilla_cupcakes",
            "{{ site.baseurl }}/baking/eclairs"
        ];
        var randomIndex = Math.floor(Math.random() * pages.length);
        location.href = pages[randomIndex];
    }
</script>
