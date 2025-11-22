# 🐦 Twimba — Mini Twitter Clone (JavaScript)



![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla-yellow)
![UUID](https://img.shields.io/badge/UUID-v4-blueviolet)
![Status](https://img.shields.io/badge/Project-Frontend%20Only-brightgreen)
![License](https://img.shields.io/badge/License-MIT-blue)


**Twimba** is a lightweight Twitter-style microblogging app built entirely with **vanilla JavaScript**.  
It allows users to **post tweets, like, retweet, and view replies** — all without a backend.  
The UI updates dynamically using DOM manipulation and a simple local dataset.

---

## 🚀 Features

- ✍️ **Post tweets** in real time  
- ❤️ **Like / Unlike** tweets  
- 🔁 **Retweet / Undo Retweet**  
- 💬 **Show / Hide replies**  
- ⚡ **Instant DOM rendering** using template strings  
- 🆔 **Unique tweet IDs** generated via `uuidv4()`  
- 📦 **In-memory data model** stored in `tweetsData`

---

## 🧩 How It Works

The app listens for *all clicks* using:

```js
document.addEventListener('click', function(e) { ... })
```

| Attribute             | Purpose                   |
| --------------------- | ------------------------- |
| `data-like="uuid"`    | ❤️ Like / Unlike a tweet  |
| `data-retweet="uuid"` | 🔁 Retweet / Undo retweet |
| `data-reply="uuid"`   | 💬 Show / hide replies    |
| `id="tweet-btn"`      | ✍️ Post a new tweet       |


## 🔄 UI Re-Rendering
After any interaction, the UI is refreshed using:

```
render()
```

## 🏗️ Constructing the Feed
The tweets are generated from tweetsData using the function:
```
getFeedHtml()
```

This builds the tweet HTML structure (likes, retweets, replies) and injects it into:
```
<div id="feed"></div>
```
## 📦 Tech Stack

- Vanilla JavaScript

- HTML / CSS

- Font Awesome (icons)

- uuid (uuidv4() for unique IDs)

📁 Project Structure
/project
│── index.html

│── index.css

│── index.js  ← (main logic)

│── data.js   ← tweet dataset

│── images/


## ▶️ How to Run

- Download or clone the project

- Open index.html in your browser

- Start tweeting 🎉

- No build tools. No backend. 100% client-side.