# অপারেটর প্রেসিডেন্স

সাধারণ গণিতে যেমন যোগ বা বিয়োগের আগে গুন ও ভাগ করে নিতে হয় তেমনি প্রোগ্রামিং -এও এই অপারেটর গুলোর একটা অগ্রাধিকার মূলক নিয়ম আছে। অর্থাৎ সেই নিয়ম মেনেই একটি স্টেটমেন্ট এর মধ্যে থাকা একাধিক অপারেটরের অপারেশন ঘটবে। এটা গণিতের সরল করার নিয়মের সাথেই মিলে যায় অর্থাৎ - প্রথমেই ব্র্যাকেটের কাজ, তারপর পাওয়ার/এক্সপোনেন্ট, অতঃপর গুন ও ভাগ এবং শেষে যোগ ও বিয়োগ।

যোগ, বিয়োগ, গুন, ভাগ বাদেও যেহেতু প্রোগ্রামিং -এ আরও কিছু অপারেটর আছে, তাই সেগুলোর অগ্রাধিকারও জেনে রাখা দরকার। যেমন নিচের স্টেটমেন্ট দুটি দেখি,

```python
>>> False == False or True
True
>>> False == (False or True)
False
```

উপরের প্রথম স্টেটমেন্টে `==` এর অগ্রাধিকার `or` চেয়ে বেশি। আর নিচের স্টেটমেন্টে `or` অপারেশন অগ্রাধিকার পেয়েছে কারন এটি একটি বন্ধনীর মধ্যে অবস্থান করছে।

| অপারেটর |
| :--- |
| `**` |
| `~+-` |
| `* / % //` |
| `+-` |
| `>> <<` |
| `&` |
| `^` |
| `<= < > >=` |
| `<> == !=` |
| `= %= /= //= -= += *= **=` |
| `is is not` |
| `in not in` |
| `not or and` |

টেবিলঃ বিভিন্ন অপারেটরের অগ্রাধিকার \(উপর থেকে নিচে - বেশি থেকে কম\)

