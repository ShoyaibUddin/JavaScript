# Class

জাভাস্ক্রিপ্ট ক্লাস হল অবজেক্ট-ওরিয়েন্টেড প্রোগ্রামিংয়ের একটি গুরুত্বপূর্ণ ধারণা যা আমাদেরকে একই ধরনের অবজেক্টগুলির ব্লুপ্রিন্ট তৈরি করতে সাহায্য করে। এটি কোডকে আরও সুসংগঠিত, পুনর্ব্যবহারযোগ্য এবং বোধগম্য করে তোলে।

**কেন ক্লাস ব্যবহার করবেন?**

- কোডের পুনর্ব্যবহারযোগ্যতা: একবার একটি ক্লাস তৈরি করলে, আপনি তার অনেকগুলি ইনস্ট্যান্স তৈরি করতে পারেন।
- কোডের সুসংগতি: ক্লাসগুলি কোডকে আরও সুসংগঠিত করে এবং বোঝা সহজ করে।
- ইনহেরিটেন্স: ক্লাসগুলি ইনহেরিটেন্সকে সমর্থন করে, যার ফলে আপনি একটি ক্লাস থেকে অন্য একটি ক্লাস তৈরি করতে পারেন এবং তার প্রপার্টি ও মেথডগুলো ব্যবহার করতে পারেন।
- পলিমরফিজম: ক্লাসগুলি পলিমরফিজমকে সমর্থন করে, যার ফলে আপনি একই নামের মেথডগুলোকে বিভিন্ন ক্লাসে ভিন্নভাবে বাস্তবায়ন করতে পারেন।

```
class Car {
  constructor(brand, model) {
    this.brand = brand;
    this.model = model;
  }

  start() {
    console.log("Car started");
  }
}
```

**একটি ক্লাসের ইনস্ট্যান্স তৈরি করা**

```
const myCar = new Car("Toyota", "Camry");
myCar.start(); // Output: "Car started"
```

### ইনহেরিটেন্স

```
class ElectricCar extends Car {
  constructor(brand, model, battery) {
    super(brand, model);
    this.battery = battery;
  }

  charge() {
    console.log("Car is charging");
  }
}
```
