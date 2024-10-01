# JavaScript Object Definition

Object হল জাভাস্ক্রিপ্টের এক ধরনের ডাটা স্ট্রাকচার যেখানে আমরা কিছু নির্দিষ্ট তথ্য বা ডাটা একসাথে রাখতে পারি। এই তথ্যগুলোকে প্রপার্টি বলা হয় এবং প্রপার্টিগুলোর সাথে যুক্ত ফাংশনগুলোকে মেথড বলা হয়।

#### Methods for Defining JavaScript Objects

- Using an Object Literal
- Using the new Keyword
- Using an Object Constructor
- Using Object.assign()
- Using Object.create()
- Using Object.fromEntries()

1. Object Literal ব্যবহার করে:

   এটি অবজেক্ট তৈরির সবচেয়ে সাধারণ এবং সহজ পদ্ধতি। এখানে আমরা কেবলই কার্লি ব্র্যাকেটের মধ্যে প্রপার্টি এবং মেথডগুলো লিখি।

   > An object literal is also callled an object initializer.

```
let person = {
  firstName: "আবুল",
  lastName: "কাশেম",
  age: 30,
  city: "ঢাকা"
};
```

2. new Keyword ব্যবহার করে:
   এখানে আমরা একটি কনস্ট্রাক্টর ফাংশন তৈরি করি এবং তারপর new কিওয়ার্ড ব্যবহার করে অবজেক্ট তৈরি করি।

```
function Person(firstName, lastName, age) {
  this.firstName = firstName;
  this.lastName = lastName;
  this.age = age;
}

let person = new Person("আবুল", "কাশেম", 30);

```

3. Object Constructor ব্যবহার করে:
   এটি new কিওয়ার্ড ব্যবহারের মতোই কাজ করে। তবে এখানে আমরা Object কনস্ট্রাক্টরকে প্রোটোটাইপ হিসেবে ব্যবহার করি।

```
let person = new Object();
person.firstName = "আবুল";
person.lastName = "কাশেম";
person.age = 30;
```

4. Object.assign() ব্যবহার করে:
   এই পদ্ধতিটি একটি ইক্সিস্ট করা অবজেক্টকে অন্য একটি অবজেক্টের প্রপার্টি দিয়ে আপডেট করতে ব্যবহৃত হয়।

```
let person = { firstName: "আবুল" };
Object.assign(person, { lastName: "কাশেম", age: 30 });
```

5. Object.create() ব্যবহার করে:
   এই পদ্ধতিটি একটি নতুন অবজেক্ট তৈরি করে এবং তার প্রোটোটাইপ হিসেবে অন্য একটি অবজেক্টকে সেট করে।

```
let personProto = {
  greet: function() {
    console.log("Hello");
  }
};

let person = Object.create(personProto);
person.name = "আবুল";

```

6. Object.fromEntries() ব্যবহার করে:
   এই পদ্ধতিটি একটি এন্ট্রি এর একটি এরে থেকে একটি নতুন অবজেক্ট তৈরি করে।

```
let entries = [
  ['name', 'আবুল'],
  ['age', 30]
];

let person = Object.fromEntries(entries);
```

### কোন পদ্ধতিটি ব্যবহার করবেন?

- Object Literal: সহজ এবং সাধারণ অবজেক্ট তৈরির জন্য।
- new Keyword: কনস্ট্রাক্টর ফাংশন ব্যবহার করে অবজেক্ট তৈরির জন্য।
- Object Constructor: প্রোটোটাইপ ব্যবহার করে অবজেক্ট তৈরির জন্য।
- Object.assign(): একটি ইক্সিস্ট করা অবজেক্টকে আপডেট করার জন্য।
- Object.create(): প্রোটোটাইপ চেইন ব্যবহার করে অবজেক্ট তৈরির জন্য।
- Object.fromEntries(): এন্ট্রি এর একটি এরে থেকে অবজেক্ট তৈরির জন্য।
