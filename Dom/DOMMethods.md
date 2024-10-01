# HTML DOM Methods

### মূল ধারণাগুলো:

- মেথড: এগুলো হল HTML এলিমেন্টগুলোর উপর আপনি যেসব অ্যাকশন করতে পারেন। এগুলো DOM স্ট্রাকচার বা বিহেভিয়ার পরিবর্তন করতে দেয়।

  > > উদাহরণ: createElement, appendChild, removeChild, setAttribute, removeAttribute.

- প্রপার্টি: এগুলো হল HTML এলিমেন্টগুলোর সাথে যুক্ত মান। এগুলো এলিমেন্টগুলোর বৈশিষ্ট্য বা অ্যাট্রিবিউট প্রকাশ করে।
  > > উদাহরণ: innerHTML, className, style, href.

### জাভাস্ক্রিপ্ট দিয়ে DOM-এ অ্যাক্সেস করা:

```
// এলিমেন্টগুলোতে অ্যাক্সেস করা
const heading = document.getElementById("myHeading");
const paragraph = document.querySelector(".paragraph");

// প্রপার্টিগুলো পরিবর্তন করা
heading.innerHTML = "নতুন হেডিং";
paragraph.style.color = "লাল";

// নতুন এলিমেন্ট যোগ করা
const newParagraph = document.createElement("p");
newParagraph.textContent = "এটি একটি নতুন প্যারাগ্রাফ।";
document.body.appendChild(newParagraph);

// এলিমেন্টগুলো মুছে ফেলা
const elementToRemove = document.querySelector("p");
elementToRemove.remove();

```
