# Creating New HTML Elements (Nodes)

এখানে আমরা জাভাক্রিপের মাধ্যমে

```
<script>
const para = document.createElement("p");
const node = document.createTextNode("This is new.");
para.appendChild(node);

const element = document.getElementById("div1");
element.appendChild(para);
</script>

```
