# Zomato Clone

> A responsive food-delivery landing page built with plain HTML, CSS and JavaScript — no frameworks, no build step.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## Overview

Zomato Clone recreates the look and feel of the Zomato home page: a red-branded header, a hero section with a search bar, and a "Why Choose Us" section with feature cards. It is written in vanilla HTML, CSS and JavaScript, which makes it a compact reference for semantic markup, Flexbox layouts, responsive design and small DOM interactions.

## Features

- **Branded header and navigation** — Zomato-red (`#e23744`) bar with the logo and links to Investor Relations, Add Restaurant, Login and Signup, each with a hover highlight.
- **Hero section with search** — full-width food photo with a dark overlay for readable text, a location tagline and a prominent search bar for restaurants, cuisines and dishes.
- **Animated search input** — JavaScript smoothly resizes the search bar when it gains or loses focus.
- **"Why Choose Us" feature cards** — Fast Delivery, Variety of Choices and Easy Payment cards that lift on hover.
- **Responsive layout** — Flexbox plus a `768px` breakpoint: the header stacks and the cards resize for tablets and phones.
- **Semantic, accessible markup** — `<header>`, `<nav>`, `<main>`, `<section>` and `<footer>` elements, `alt` text on images and an `aria-label` on the search field.
- **Zero dependencies** — open `index.html` and it works.

## Screenshot

![Zomato Clone home page](docs/screenshot.png)

*Home page, desktop view (1280 px wide).*

## Tech Stack

| Category  | Technology                                                       |
| --------- | ---------------------------------------------------------------- |
| Markup    | HTML5 (semantic elements)                                        |
| Styling   | CSS3 — Flexbox, media queries, transitions, `::before` overlay   |
| Scripting | Vanilla JavaScript (ES6, DOM events)                             |
| Tooling   | None — runs directly in any modern browser                       |

## Installation

There are no dependencies to install — just a modern web browser and Git.

```bash
# Clone the repository
git clone https://github.com/vinayakmishra4/ZOMATO-CLONE.git

# Move into the project folder
cd ZOMATO-CLONE
```

## Usage

**Option 1 — open the file directly**

```bash
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

**Option 2 — run a local server (recommended)**

```bash
python3 -m http.server 8000    # use `python` on Windows
```

Then visit <http://localhost:8000>. Alternatively, use the **Live Server** extension in VS Code and click *Go Live*.

**What to try**

- Hover over the navigation links — they turn gold.
- Click into the search bar to see the focus animation.
- Hover over the feature cards to see them lift.
- Resize the browser below 768 px to see the responsive layout.

**Customising**

The tagline and city are set in the hero section of `index.html`:

```html
<p>Discover the best food &amp; drinks in Hanumangarh</p>
```

The primary brand colour (`#e23744`) and all layout rules live in `css/style.css`.

> [!NOTE]
> The navigation links (Investor Relations, Add Restaurant, Login, Signup) point to pages that are not built yet. See [Future Improvements](#future-improvements).

## Project Structure

```text
ZOMATO-CLONE/
├── css/
│   └── style.css          # Theme, layout, hover effects, responsive rules
├── docs/
│   └── screenshot.png     # Screenshot used in this README
├── image/
│   ├── bg.png             # Hero section background
│   ├── logo.png           # Logo used in the header and hero
│   └── Zomato_logo.png    # Additional logo asset
├── js/
│   └── script.js          # Search bar focus/blur animation
├── index.html             # Home page
├── LICENSE                # MIT License
└── README.md              # You are here
```

## Future Improvements

1. **Build the pages the navbar links to** — `login.html`, `signup.html`, `add-restaurant.html` and `investor.html`.
2. **Make search functional** — load restaurants and dishes from a JSON file and filter results as the user types, then move to a real API.
3. **Add restaurant listings and ordering** — restaurant cards, menu pages and a simple cart and checkout flow.

## Disclaimer

This is a non-commercial learning project. Zomato's name and logo are trademarks of their respective owners, and this project is not affiliated with or endorsed by Zomato.

## Author

**Vinayak Mishra** — [@vinayakmishra4](https://github.com/vinayakmishra4)

## License

Distributed under the MIT License. See [LICENSE](LICENSE) for details.