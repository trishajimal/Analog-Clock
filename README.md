# Analog Clock

A simple analog clock built with HTML, CSS, and JavaScript. The clock displays the current local time with moving hour, minute, and second hands.

## Features

- Real-time analog clock display
- Hour hand movement accounts for the current minutes
- Responsive clock face sized relative to the viewport
- No frameworks or dependencies

## Run Locally

1. Clone or download this repository.
2. Open `index.html` in a web browser.

For the best development experience, open the project in VS Code and use a local server extension such as Live Server.

## Project Structure

```text
.
├── index.html   # Clock markup
├── style.css    # Clock face and hand styling
├── script.js    # Time calculations and hand rotation
├── clock.png    # Clock face image
└── README.md    # Project documentation
```

## How It Works

The JavaScript reads the current time every second and converts each value into a rotation angle:

- Hour hand: `30 × hours + minutes ÷ 2`
- Minute hand: `6 × minutes`
- Second hand: `6 × seconds`

The hands are rotated using CSS transforms around their bottom edge.
