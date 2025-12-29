# stream-tools

A small collection of stream screens implemented as plain HTML, CSS, and minimal JavaScript.

stream-tools exists to make common stream intermissions boring, predictable, and self-hostable. No build step, no frameworks, no accounts, no tracking. Just static files rendered by the browser.

The intended deployment target is GitHub Pages (or any other static host). The intended consumer is software that can display a web page, such as OBS via a Browser Source.


---

### What this is
- "Starting Soon", "Be Right Back", "Ending", and similar stream screens
- Implemented using vanilla HTML/CSS/JS
- Served as static pages
- Designed to be embedded, not interacted with

### What this is not
- A streaming platform
- A SaaS product
- A widget marketplace
- A real-time overlay system
- A framework

---

### Why

Most stream intermission screens are either:
- Locked behind proprietary tools
- Locked behind paywalls
- Animated via heavyweight runtimes
- Impossible to self-host cleanly

stream-tools takes the opposite approach: static assets, minimal logic, and full user control.

If you can host a website, you can run this.

---

## Usage

### 1. Fork or clone

Fork this repository, or clone it locally if you plan to customize.

git clone https://github.com/SleepingAmi/stream-tools.git

### 2. Enable hosting

Enable GitHub Pages (or equivalent) and point it at the repository root.

Once enabled, each screen will be accessible as a normal URL, usually at your-username.github.io/stream-tools.

### 3. Add to OBS

In OBS:

1. Add a Browser Source
2. Set the URL to the page you want (e.g. stream-tools/starting-soon)
3. Set width/height to your canvas resolution
4. Enable cache refreshing or similar, if applicable (sometimes animation are cached and break the layout)

No local files are required on the streaming machine, unless you rawdog "From source file" in OBS.

---

## Customisation

Customisation is expected.

Each screen is intentionally simple:
- Text can be changed directly in HTML
- Colours, fonts, and layout live in CSS
- Animations (where present) are implemented in plain CSS
- Timers (where present) are implemented in plain JS

There is no configuration system. Edit the files.

If you are comfortable with web basics, nothing here should be surprising.

---

## Screens

Available screens typically include:
- Starting Soon
- Be Right Back
- Ending
- Technical Difficulties

<!-- Exact filenames and features are documented inline in each screen's directory. -->

Screens are independent. You can delete the ones you do not need.

---

## Browser compatibility

Targets modern Chromium-based browsers, as used by OBS Browser Source.

No attempt is made to support legacy browsers.

---

## Contributing

Contributions are welcome, provided they follow the project's constraints:
- No external frameworks
- No build tooling
- No trackers, analytics, or third-party calls
- Keep it static
- Keep it readable

New screens, refinements, and bug fixes are all acceptable.

If a change increases complexity without a clear benefit, it will likely be rejected.

---

## License

Licensed under the [MIT License](https://mit-license.org/).


---

## Notes

If you are looking for something dynamic, managed, or interactive, this project is probably not what you want.

This is a free product that happens to be implemented as static files.
