console a যদি document.dir(কোন এলিমেন্ট দেওয়া হয়) তাহলে ওই এলিমেন্টর বিস্তারিত দেখা যাবে।

# যা যা শিখলাম তা এক নজরে।

```
const x = document.forms["frm1"];

let text = "";

for (let i=0; i< x.length; i++) {
    text += x.elements[i].value + "<br>";
}


document.getElementById("jan").innerHTML = text;
```

```
document.getElementById("main");
document.getElementsByClassName("");
querySelectorAll()
document.getElementsByTagName(name)
```

> In the example above, getElementById is a method, while innerHTML is a property.

- querySelector() এখানে এখই রকমের জিনিসের প্রথম এলিমেন্ট টা ধরে।
- querySelectorAll() এটার মাধ্যমে সব কয়টি এলিমেন্ট ধরে। ‍কিন্তু লুপের মাধ্যমে প্রতিটি তে style Add করতে হয়।
  [Ref](https://youtu.be/HSi3WYjt12Q?t=1187)

## Changing HTML

```
document.write();
```

## form validation

```
function haha() {
    const mi =  document.getElementById("frm1");
    let ys = mi['fname'].value;

    if (ys == "") {
        alert("Sramm a");

        return false;
    }
}
```

# CSS change

[Ref:](https://youtu.be/g1W_ixdu8U8?list=PLHiZ4m8vCp9OkrURufHpGUUTBjJhO9Ghy)

```
p.style.color = "red";
p.style.fontFamily = "";
```

SetTimeout -

```
setTimeout (function(){

}, 2000);
```

## Traversing DOM

✅ .getElementById<br>
✅ .getElementsByClassName<br>
✅ .getElementsByTagName<br>
✅ .textContent<br>
✅ .innerText<br>
✅ .innerHTML<br>
✅ .querySelector<br>
✅ .querySelectorAll<br>
✅ .children<br>
✅ .parent<br>
✅ .closest<br>
✅ .nextElementSibling<br>
✅ .previousElementSibling<br>

## [Manipulate the DOM](https://youtu.be/NmInTfiUcw0)

### Creating an element

.createElement() <br>
.className = <br>
.setAttribute ('title', "red"); [ref](https://youtu.be/NmInTfiUcw0?t=334) <br>
.insertBefore(newElemnt, যার আগে বসাবে); <br>
.appendChild();এটায় অবশ্যই HTML এলিমেন্ট দিতে হবে<br>
.append(); এটিতে টেক্স এলিমেন্ট দেয়া যায়।

.append(মাল্টিপল প্যরামিটারের মাধ্যমে এলিমেন্ট দেওয়া যায়);
