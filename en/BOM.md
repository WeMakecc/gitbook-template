# BOM {#bom}

This is a template for a BOM list.

> The following layout requires the [`layout-tags`](https://github.com/WeMakecc/gitbook-plugin-layout-tags) plugin

It is possible to have BOM list layout with the following syntax:
```
{% bom %}
    {% bom_image "potentiometer", "70px", "left", "margin-right:10px" %}../assets/pot.jpg
    {% bom_description %}10k Potentiometer
    {% bom_quantity %}X 5
{% endbom %}

---

{% bom %}
    {% bom_image "resistor", "70px", "left", "margin-right:10px" %}../assets/resistor.jpg
    {% bom_description %}100ohm Resistors
    {% bom_quantity %}X 10
{% endbom %}

---

{% bom %}
    {% bom_image "capacitor", "70px", "left", "margin-right:10px" %}../assets/capacitor.jpg
    {% bom_description %}4700uF Capacitors
    {% bom_quantity %}X 2
{% endbom %}

---
```

See result:

{% bom %}
    {% bom_image "potentiometer", "70px", "left", "margin-right:10px" %}../assets/pot.jpg
    {% bom_description %}10k Potentiometer
    {% bom_quantity %}X 5
{% endbom %}

---

{% bom %}
    {% bom_image "resistor", "70px", "left", "margin-right:10px" %}../assets/resistor.jpg
    {% bom_description %}100ohm Resistors
    {% bom_quantity %}X 10
{% endbom %}

---

{% bom %}
    {% bom_image "capacitor", "70px", "left", "margin-right:10px" %}../assets/capacitor.jpg
    {% bom_description %}4700uF Capacitors
    {% bom_quantity %}X 2
{% endbom %}

---


**_IMPORTANT_** It is very important to note:
- all tags are needed to be filled and displayed, removing one of the tags would turn into a display error


> It's possible to achieve the same layout without using the `layout-tags` with a table layout:
```markdown
|Item|Description|Quantity|
|-|-|-|
|![](../assets/pot-small.jpg)|10k Potentiometer|x 5|
|![](../assets/resistor-small.jpg)|100ohm Resistor|x 10|
```

See result:
|Item|Description|Quantity|
|-|-|-|
|![](../assets/pot-small.jpg)|10k Potentiometer|x 5|
|![](../assets/resistor-small.jpg)|100ohm Resistor|x 10|


**_IMPORTANT_** It is very important to note:
- don't write any text in the alternative text section of the image as it would break the layout! (eg. please avoid the following markdown `![potentiometer](../assets/pot-small.jpg)`)














