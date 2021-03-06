# বুলিয়ান

বুলিয়ান হলো এক প্রকারের ডাটাটাইপ যার মান সবসময় কোন কিছু সত্য অথবা মিথ্যা বুঝায়। সত্য ও মিথ্যাকে যথাক্রমে 1 ও 0 দ্বারা প্রকাশ করা হয়। এটি ইন্টেজার এর একটি সাবক্লাস। বুলিয়ান ধারনার প্রবক্তা জর্জ বুল। তার বই ‘দা ম্যাথমেটিকাল এনালাইসিস অফ লজিক\(১৮৪৭\)’ থেকে সর্বপ্রথম এ সম্পর্কে ধারনা পাওয়া যায়।

পাইথনে এই Boolean টাইপটির দুটি ভ্যালু আছে `True` এবং `False`

**বুলিয়ান এক্সপ্রেশন**  
বুলিয়ান এক্সপ্রেশন হলো এমন কিছু এক্সপ্রেশন যেগুলো সত্য অথবা মিথ্যা মান রিটার্ন করে। একাধিক বুলিয়ান এক্সপ্রেশন মিলেও একটি বুলিয়ান এক্সপ্রেশন বানানো যায়।

**বুলিয়ান অপারেটর**  
বুলিয়ান টাইপের তিনটি বেসিক অপারেটর আছে। এরা হলো `AND` , `OR` , `NOT`। `AND` এর বেলায় যদি সবগুলো ভ্যারিয়েবল এর মান সত্য হয় তবে এক্সপ্রেশন টি সত্য হয় অন্যথায় এক্সপ্রেশন টি মিথ্যা হয়। `OR` এর বেলায় যদি কমপক্ষে একটি ভ্যারিয়েবল এর মান সত্য হয় তবে এক্সপ্রেশন টি সত্য হয় অন্যথায় এক্সপ্রেশন টি মিথ্যা হয়। `NOT` একটি ইউনারি অপারেটর। এটি সাধারনত কোনো ভ্যারিয়েবল অথবা এক্সপ্রেশন এর বিপরীত ভ্যালু রিটার্ন করে।

**ট্রুথ টেবিল**  
নিচে ট্রুথ টেবিল এর মাদ্ধ্যমে বিষয়গুলো তুলে ধরা হলোঃ-

| A | B | A AND B | A OR B | NOT A |
| :--- | :--- | :--- | :--- | :--- |
| 0 | 0 | 0 | 0 | 1 |
| 0 | 1 | 0 | 1 | 1 |
| 1 | 0 | 0 | 1 | 0 |
| 1 | 1 | 1 | 1 | 0 |

এই বেসিক এপারেটর ছাড়াও আরো কিছু অপারেটর আছে যেগুলো এই তিনটির সনন্বয়ে গঠন করা হয়েছে। যেমনঃ `XOR`,`XAND`,`NAND`,`NOR` ইত্যাদি। এ নিয়ে সামনের কোন এক চ্যাপ্টারে আবারো আলোচনা হবে।

**পাইথনে কিছু উদাহরণ**  
পাইথনে দুটো এলিমেন্ট এর মধ্যে তুলনা করে অথবা সরাসরি ভ্যালু অ্যাসাইন করে বুলিয়ান ভ্যারিয়েবল তৈরি করা যায়। যেমন,

```python
>>> my_boolean = True
>>> my_boolean
True

>>> 2 == 3
False
>>> "hello" == "hello"
True
```

আরও কিছু তুলনাকারী অপারেটর ব্যবহারের সময়,

```python
>>> 1 != 1 # দেখা হচ্ছে ১ নট ইকুয়াল ১ কিনা। যেটা আসলে মিথ্যা। বাস্তবে ১ ইকুয়াল ১
False
>>> "eleven" != "seven" # এখানে eleven আর seven ইকুয়াল নয়। তাই এটা সত্য 
True
>>> 2 != 10 # ২ কিন্তু ১০ এর সমান নয় যেটা যাচাই করা হচ্ছে। তাই যাচাই এর মান সত্য 
True
```

```python
>>> 7 > 5
True
>>> 10 < 10
False
>>> 7 <= 8
True
>>> 9 >= 9.0
True
```

