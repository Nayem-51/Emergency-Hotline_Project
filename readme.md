# 📘 Assignment-005

This is my project submission for **Assignment-005**.  
I have implemented the required features using **HTML, CSS (Tailwind CSS), and Vanilla JavaScript**.

---

## ✨ Features
- Navbar with logo, heart icon, coin counter, and copy counter  
- Hero Section with background gradient, logo, title, and slogan  
- Emergency Hotline Cards with call and copy buttons  
- Call History Section with clear history button  
- Responsive design for mobile devices  
- Functionalities: Like (heart), Call (with coin deduction), Copy, and History tracking  

---

## 📝 Questions & Answers

### 1. What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?

- **getElementById** → নির্দিষ্ট একটা element কে তার `id` দিয়ে ধরতে ব্যবহার হয়। এটা সবসময় একটা element রিটার্ন করে।  
- **getElementsByClassName** → একই class নাম থাকা একাধিক element ধরতে ব্যবহার হয়। এটা HTMLCollection (array-like) রিটার্ন করে।  
- **querySelector** → CSS selector দিয়ে element ধরতে পারে। কিন্তু শুধু প্রথম matching element টা রিটার্ন করে।  
- **querySelectorAll** → CSS selector দিয়ে সব matching element ধরে এবং NodeList আকারে রিটার্ন করে।  

---

### 2. How do you create and insert a new element into the DOM?

1. **নতুন element তৈরি করা**:  
   ```js
   const newDiv = document.createElement("div");
   ```
2. **কিছু কনটেন্ট যোগ করা**:  
   ```js
   newDiv.textContent = "Hello World!";
   ```
3. **DOM এ append করা**:  
   ```js
   document.body.appendChild(newDiv);
   ```

এভাবে আমরা নতুন element তৈরি করে ওয়েবপেজে যোগ করতে পারি।

---

### 3. What is Event Bubbling and how does it work?

Event bubbling মানে হলো যখন একটা event (যেমন click) কোনো element এ ঘটে, তখন সেটা প্রথমে সেই element এ কাজ করে, তারপর parent → grandparent → document পর্যন্ত উপরের দিকে propagate হয়।  
Example: যদি একটা button এর ভেতরে একটা div থাকে, আর div এর ভেতরে একটা click listener থাকে, button এ ক্লিক করলে event প্রথমে button → div → body → document এ চলে যাবে।

---

### 4. What is Event Delegation in JavaScript? Why is it useful?

Event Delegation মানে হলো parent element এ event listener বসানো, আর child element গুলোর event ওই parent এর মাধ্যমে handle করা।  
এটা useful কারণ:  
- অনেক child element এর জন্য আলাদা আলাদা listener বসাতে হয় না।  
- Dynamic element (যেগুলো পরবর্তীতে DOM এ যোগ হয়) সেগুলোও সহজে handle করা যায়।  

---

### 5. What is the difference between preventDefault() and stopPropagation() methods?

- **preventDefault()** → ব্রাউজারের default action বন্ধ করে। যেমন form submit করলে page reload হয়, সেটা বন্ধ করতে।  
- **stopPropagation()** → event bubbling বা capturing বন্ধ করে দেয়। মানে event আর parent element এ propagate হবে না।  

---

## 🚀 Technology Stack
- HTML  
- CSS (TailwindCSS)  
- JavaScript (Vanilla)  

---
