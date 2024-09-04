---
layout: page
title: Savory Recipes
permalink: /savory/
---

### Savory Recipes To Bake

<div style="text-align: center; margin-top: 20px;">
    <img src="{{ site.baseurl }}/images/sweet_treats.png" style="max-width: 100%; border-radius: 15px; box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);">
</div>

<div style="text-align: center; margin-top: 20px;">
    <select id="baking-menu" style="padding: 10px; border-radius: 5px; border: 1px solid #ccc; background-color: #f8f8f8;" onchange="location = this.value;">
        <option value="">Select a dish</option>
        <option value="{{ site.baseurl }}/sweet/choco_chip_cookies">Choco Chip Cookies</option>
        <option value="{{ site.baseurl }}/sweet/vanilla_layer_cakes">Vanilla Layer Cake</option>
        <option value="{{ site.baseurl }}/sweet/sugar_cookies">Sugar Cookies</option>
        <option value="{{ site.baseurl }}/sweet/lava_cakes">Lava Cake</option>
        <option value="{{ site.baseurl }}/sweet/vanilla_cupcakes">Vanilla Cupcakes</option>
        <option value="{{ site.baseurl }}/sweet/eclairs">Eclairs</option>
        <option value="javascript:randomPage()">Wildcard</option>
    </select>
</div>

<script>
    function randomPage() {
        var pages = [
            "{{ site.baseurl }}/sweet/choco_chip_cookies",
            "{{ site.baseurl }}/sweet/vanilla_layer_cakes",
            "{{ site.baseurl }}/sweet/sugar_cookies",
            "{{ site.baseurl }}/sweet/lava_cakes",
            "{{ site.baseurl }}/sweet/vanilla_cupcakes",
            "{{ site.baseurl }}/sweet/eclairs"
        ];
        var randomIndex = Math.floor(Math.random() * pages.length);
        location.href = pages[randomIndex];
    }
</script>
