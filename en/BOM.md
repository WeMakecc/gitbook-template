# BOM {#bom}

This is a template for a BOM list.

{% bom %}
    {% bom_image "potentiometer", "70px", "left", "margin-right:10px" %}../assets/pot.jpg
    {% bom_description %}10k Potentiometer
    {% bom_quantity %}5x
{% endbom %}

---

{% image %}
    {% image_url "resistor", "70px", "left", "margin-right:10px" %}../assets/resistor.jpg
    {% image_text %}10x 100ohm Resistors
{% endimage %}

---

{% image %}
    {% image_url "capacitor", "70px", "left", "margin-right:10px" %}../assets/capacitor.jpg
    {% image_text %}2x 4700uF Capacitors
{% endimage %}

---

|Item|Description|Quantity|
|-|-|-|
|![](../assets/pot-small.jpg)|10k Potentiometer|x 5|
|![](../assets/resistor-small.jpg)|100ohm Resistor|x 10|

---

|Item|Description|Quantity|
|-|-|-|
|pic|description|5|
|pic|item description|10|






