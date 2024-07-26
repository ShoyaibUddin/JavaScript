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

✅ .getElementById
✅ .getElementsByClassName
✅ .getElementsByTagName
✅ .textContent
✅ .innerText
✅ .innerHTML
✅ .querySelector
✅ .querySelectorAll
✅ .children
✅ .parent
✅ .closest
✅ .nextElementSibling
✅ .previousElementSibling
