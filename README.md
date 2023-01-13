<h1 align='center'>খুব সহজে শিখবো ও জানবো সিএসস  ফ্লেক্স বক্স সম্পর্কে 😀</h1>

### Description In Flex Box ☐

CSS Flexbox হল CSS-এর একটি লেআউট মডিউল যা আপনাকে ন্যূনতম কোড সহ সহজেই নমনীয়, প্রতিক্রিয়াশীল এবং অভিযোজিত লেআউট তৈরি করতে দেয়। এটি একটি পাত্রের মধ্যে আইটেমগুলিকে সারিবদ্ধ করার এবং বিতরণ করার একটি উপায় প্রদান করে, এবং উপাদানগুলির জন্য স্বয়ংক্রিয়ভাবে ধারকটির আকার এবং এর মধ্যে থাকা উপাদানগুলির উপর ভিত্তি করে পুনরায় আকার এবং পুনরায় অবস্থান করার অনুমতি দেয়৷ ফ্লেক্সবক্স কলাম, সারি, গ্রিড এবং আরও অনেক কিছু সহ বিভিন্ন লেআউট প্যাটার্ন তৈরি করতে ব্যবহার করা যেতে পারে Css FlexBox।


![flex-box](https://user-images.githubusercontent.com/106922916/212260471-a851b6e3-6d60-4d97-81aa-f383bdf02e42.png)


[//]: # (Table of Content)

<a name="top"></a>

## Table of FlexBox All content

> Click on any topic to go there
- [Flexbox Architecture 🎖️](#flex-1)
- [All CSS Flexbox properties 🎖️](#flex-2)
- [Flexbox Chart 🎖️](#flex-3)
- [CSS Display Flex 🎖️](#flex-4)
- [Flex Direction 🎖️](flex-5)
- [Justify Content 🎖️](flex-6)
- [Flex Align Items 🎖️](flex-7)
- [Align Self 🎖️](flex-8)
- [Flex Wrap 🎖️](flex-9)



***

### Flexbox Architecture 🎖️

<a name="flex-1"></a>

> তাহলে কিভাবে ফ্লেক্সবক্স আর্কিটেকচার কাজ করে? ফ্লেক্স-আইটেম [বিষয়বস্তু] প্রধান অক্ষ X (**Horizontal**) এবং ক্রস Y (**Vertically**) অক্ষ বরাবর বিতরণ করা হয়। এবং, ফ্লেক্স-দিক বৈশিষ্ট্যের উপর নির্ভর করে, সারি এবং কলামের মধ্যে বিন্যাসের অবস্থান পরিবর্তিত হয়।

![hy2oqjvsbk60ef92nktg](https://user-images.githubusercontent.com/106922916/212272286-90328c5d-cd6e-4ad0-9c50-cc3e633ad8a5.png)


<a name="flex-2"></a>

### All CSS Flexbox properties 🎖️

> এখানে সমস্ত সিএসএস ফ্লেক্সবক্স বৈশিষ্ট্যের একটি তালিকা রয়েছে যা CSS-এ উপাদানগুলির অবস্থানের জন্য ব্যবহার করা যেতে পারে। পরবর্তী, আপনি তারা কিভাবে কাজ দেখতে পাবেন.

#### সিএসএস যা কন্টেইনারে প্রয়োগ করা যেতে পারে

```css

display: flexbox | inline-flex;
flex-direction: row | row-reverse | column | column-reverse;
flex-wrap: nowrap | wrap | wrap-reverse;
flex-flow: <‘flex-direction’> || <‘flex-wrap’>
justify-content: flex-start | flex-end | center | space-between | space-around;
align-items: flex-start | flex-end | center | baseline | stretch;
align-content: flex-start | flex-end | center | space-between | space-around | stretch;

```

#### Css যা কন্টেইনারের আইটেম/উপাদানগুলিতে প্রয়োগ করা যেতে পারে

```css

order: <integer>;
flex-grow: <number>; /* default 0 */
flex-shrink: <number>; /* default 1 */
flex-basis: <length> | auto; /* default auto */
flex: none | [ <'flex-grow'> <'flex-shrink'>? || <'flex-basis'> ]
align-self: auto | flex-start | flex-end | center | baseline | stretch;

```

<a name="flex-3"></a>

### Flexbox Chart 🎖️

> এই চার্টে আপনি ফ্লেক্সবক্সের সাথে কাজ করার সময় ব্যবহার করতে পারেন এমন প্রতিটি সম্ভাব্য সম্পত্তি এবং মান রয়েছে। আপনি আপনার প্রকল্পগুলি করার সময় এটি উল্লেখ করতে পারেন এবং বিভিন্ন মান নিয়ে পরীক্ষা করতে পারেন।

![gv3jyh4xt4fbwtq1qejn](https://user-images.githubusercontent.com/106922916/212274426-80b91896-5d11-4b94-afd1-137cadbb5b5b.png)


<a name="flex-4"></a>

### CSS Display Flex 🎖️

> **display:flex;** আপনার ব্রাউজারকে বলে, "আমি এই ধারকটির সাথে flexbox ব্যবহার করতে চাই, দয়া করে।"

>একটি div উপাদান প্রদর্শন করতে ডিফল্ট: ব্লক। এই ডিসপ্লে সেটিং সহ একটি উপাদান এটি যে লাইনে রয়েছে তার পুরো প্রস্থটি নেয়। এখানে ডিফল্ট ডিসপ্লে সেটিং সহ একটি প্যারেন্ট ডিভ-এ চারটি রঙিন ডিভের একটি উদাহরণ রয়েছে:


![ChnkgUaWEN6dmtS4EQCG60uqIjZVphsErq91](https://user-images.githubusercontent.com/106922916/212276128-e0ff78e7-bf55-46e5-8e51-5474f16bfeaa.gif)

> আপনার পৃষ্ঠার একটি বিভাগে ফ্লেক্সবক্স ব্যবহার করতে, প্রথমে প্রদর্শন যোগ করে প্যারেন্ট কন্টেইনারটিকে একটি ফ্লেক্স কন্টেইনারে রূপান্তর করুন: flex; মূল কন্টেইনারের CSS-এ।

> এটি এই ধারকটিকে একটি ফ্লেক্স ধারক হিসাবে শুরু করবে এবং কিছু ডিফল্ট ফ্লেক্স বৈশিষ্ট্য প্রয়োগ করবে।


![6WwoIEc45lUHUcFQCmD8GmziiISm2lO64Y1-](https://user-images.githubusercontent.com/106922916/212276533-1adcae3f-a01f-400a-b701-4e00c80fd9cd.gif)


<a name="flex-5"></a>

### Flex Direction 🎖️

> ফ্লেক্স-নির্দেশ আপনাকে কন্টেইনারের আইটেমগুলি কীভাবে প্রদর্শন করবে তা নিয়ন্ত্রণ করতে দেয়। আপনি কি তাদের বাম থেকে ডানে, ডান থেকে বামে, উপরে থেকে নীচে, বা নীচে থেকে উপরে চান? আপনি ধারকটির ফ্লেক্স-দিক নির্ধারণ করে সহজেই এই সব করতে পারেন।

> ডিসপ্লে প্রয়োগ করার পরে ডিফল্ট বিন্যাস: ফ্লেক্স হল আইটেমগুলিকে প্রধান অক্ষ বরাবর বাম থেকে ডানে সাজানোর জন্য। নীচের অ্যানিমেশনটি দেখায় যখন ফ্লেক্স-নির্দেশ: কলামটি কন্টেইনার উপাদানে যোগ করা হয় তখন কী ঘটে।


![wEg7wdKEfv9-bqaiB-t9hzOapBPiqZVYNFIh](https://user-images.githubusercontent.com/106922916/212277416-050f57cd-3a69-4f49-ada2-f7320f3d1884.gif)


> You can also set flex-direction to row-reverse and column-reverse.

![zYdQGSmhtMyqcAbEUDoEehohC8E-gtgvQx6b](https://user-images.githubusercontent.com/106922916/212284340-f2921a30-0cd9-4e89-8848-aae5f16f00af.gif)


<a name="flex-6"></a>

### Justify Content 🎖️

> **justify-content** হল মূল অক্ষ বরাবর কন্টেইনারে আইটেমগুলিকে সারিবদ্ধ করার একটি সম্পত্তি (উপরের পরিভাষা চিত্র দেখুন)। বিষয়বস্তু কীভাবে প্রদর্শিত হয় তার উপর নির্ভর করে এটি পরিবর্তিত হয়। এটি আমাদের সারিগুলিতে যে কোনও খালি স্থান পূরণ করতে এবং কীভাবে আমরা এটিকে 'ন্যায়সঙ্গত' করতে চাই তা সংজ্ঞায়িত করতে দেয়।

> Here are our the most common options used to **justify-content**:

 ```css

 flex-start | flex-end | center | space-between | space-around | space-evenly;

```

> Here is what the different options look like: 👉 👇 👈

![OBGVr-DdHiQ2y9VOWuhXqXeGnFnyDSBTx7hv](https://user-images.githubusercontent.com/106922916/212286526-6524f528-961c-4cf9-90be-be4af6057dc5.gif)

> **space-between** মধ্যে আইটেম বিতরণ করে যাতে প্রথম আইটেমটি শুরুর সাথে ফ্লাশ হয় এবং শেষটি শেষের সাথে ফ্লাশ হয়। **space-around** একই রকম তবে আইটেমগুলির উভয় প্রান্তে অর্ধ-আকারের স্থান রয়েছে।


<a name="flex-7"></a>

### Flex Align Items 🎖️

> **align-items** আমাদের ক্রস অক্ষ বরাবর আইটেমগুলিকে সারিবদ্ধ করতে দেয় (উপরের পরিভাষা চিত্রটি দেখুন)। এটি বিষয়বস্তুকে ন্যায্যতা এবং আইটেমগুলিকে একসাথে সারিবদ্ধ করে ব্যবহার করে বিভিন্ন উপায়ে বিষয়বস্তুকে অবস্থান করার অনুমতি দেয়৷

> Here are the most common options used to align-items:

```css

flex-start | flex-end | center | baseline | stretch

```

> প্রসারিত কাজ করার জন্য আপনি যেভাবে আশা করবেন, উপাদানগুলির উচ্চতা একটি নির্দিষ্ট উচ্চতার পরিবর্তে স্বয়ংক্রিয়ভাবে সেট করা আবশ্যক।

> This animation shows what the options look like:

![UgsULw0Kk49l-l1wSzeurYNJKCmcA-01oE8a](https://user-images.githubusercontent.com/106922916/212288778-d2c6bc97-d9b6-4d3b-a406-b46eb0e67027.gif)


> এখন আমরা উভয়ই **justify-content** এবং **align-items** ব্যবহার করব। এটি প্রধান অক্ষ এবং ক্রস অক্ষের মধ্যে পার্থক্য দেখাবে।

![u9tCV-zRt3qpgSyNQt53e-eRz0-HIrsqqOk-](https://user-images.githubusercontent.com/106922916/212289319-8942e0d4-03a3-42e2-bf55-f7115144f376.gif)


<a name="flex-8"></a>

### Align Self 🎖️




> **align-self** আপনাকে একটি একক উপাদানের প্রান্তিককরণ সামঞ্জস্য করতে দেয়।
> **align-self** আইটেমগুলির সমস্ত একই বৈশিষ্ট্য রয়েছে।

> নিম্নলিখিত অ্যানিমেশনে, প্যারেন্ট ডিভিতে CSS **align-items:center;** এবং **flex-direction:row;** প্রথম দুটি বর্গক্ষেত্র বিভিন্ন সারিবদ্ধ-স্ব মানের মাধ্যমে চক্রাকারে।


![HbnMZT330ylw5idocqrjOfp9DrlZt9JrJm9o](https://user-images.githubusercontent.com/106922916/212291768-31df2f52-eb0d-41bd-833f-4490778ada8e.gif)


### Flex Wrap 🎖️

> ফ্লেক্সবক্স ডিফল্টরূপে সমস্ত উপাদানকে এক সারিতে ফিট করার চেষ্টা করবে। যাইহোক, আপনি **flex-wrap** প্রপার্টি দিয়ে এটি পরিবর্তন করতে পারেন। উপাদানগুলি কখন অন্য সারিতে যায় তা নির্ধারণ করতে আপনি তিনটি মান ব্যবহার করতে পারেন।

> ডিফল্ট মান হল **flex-wrap:nowrap;** এর ফলে সবকিছু বাম থেকে ডানে এক সারিতে থাকবে।

> **flex-wrap:** প্রথম সারিতে পর্যাপ্ত জায়গা না থাকলে **wrap** আইটেমগুলিকে পরবর্তী সারিতে পপ করার অনুমতি দেবে। আইটেমগুলি বাম থেকে ডানে প্রদর্শিত হবে।

> **flex-wrap:wrap-reverse;** আইটেমগুলিকে পরবর্তী সারিতে পপ করার অনুমতি দেয় তবে এবার আইটেমগুলি ডান থেকে বামে প্রদর্শিত হবে।


![flex-wrap-example](https://user-images.githubusercontent.com/106922916/212294407-85bb476f-42a7-43b9-b81d-245bce3dde41.gif)






