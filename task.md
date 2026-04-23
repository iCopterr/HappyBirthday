## Task: Birthday Surprise Website

### Objective

Create an interactive birthday webpage with multiple click stages.

---

## 🧩 Structure

### 1. Initial State

* Show a centered **gift box**
* Add text: "Click me 🎁"

---

### 2. First Click

* Hide box
* Show **cake with candles**
* Display text: "เป่าเทียน"

---

### 3. Second Click

* Change text to:
  "อธิษฐานรึยังข้าวปุ้น"
* Show a button: "อธิษฐานแล้ว"

---

### 4. Final Stage (Main Effect)

When user clicks "อธิษฐานแล้ว":

#### Animation:

* Cake **expands slightly then explodes (scale + opacity)**
* Confetti effect (optional simple div animation)

#### Show:

* Center message:

  ```
  Happy Birthday ข้าวปุ้น 🎂
  ขอให้มีความสุขมากๆนะ ❤️
  ```

  (Must be editable in HTML)

#### Show Images:

* Images appear around screen randomly
* Use multiple `<img>` elements
* Example:

  ```html
  <img src="img1.jpg" class="floating-img">
  <img src="img2.jpg" class="floating-img">
  ```

---

## 🎨 Styling

### Center Layout

* Use flexbox:

  * align center
  * justify center
  * full screen height

### Animations

* Cake pop-up:

  * scale(0) → scale(1)
* Explosion:

  * scale(1) → scale(1.5) → opacity(0)

### Floating Images

* Use `position: absolute`
* Random positions OR preset positions
* Add slight floating animation (translateY)

---

## 🛠 Editable Section (IMPORTANT)

Put this at the top of HTML:

```html
<!-- ===== EDIT HERE ===== -->
<h1 id="birthdayMessage">
  Happy Birthday ข้าวปุ้น 🎂
  ขอให้มีความสุขมากๆนะ ❤️
</h1>

<img src="img1.jpg">
<img src="img2.jpg">
<img src="img3.jpg">
<!-- ===================== -->
```

---

## ⚙️ Constraints

* No frameworks (React, Vue, etc.)
* Pure HTML/CSS/JS only
* Must run by opening `index.html`

---

## 💡 Bonus (Optional)

* Add sound when cake explodes 🎉
* Add glow effect on candles
* Add typing animation for message

---

## ✅ Deliverable

* 1 HTML file
* Fully working interaction
* Clean and commented code
