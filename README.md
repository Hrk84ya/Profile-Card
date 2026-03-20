# Profile Card Project

## Project Overview
A premium, dark-themed profile card built with modern CSS. Features an animated gradient border, frosted glass effect, and a warm amber/gold color scheme. Designed for personal websites, portfolios, or digital resumes.

### Check out the live demo: [Profile-Card](https://hrk84ya.github.io/Profile-Card/)

## Key Features
- Dark theme with deep `#0f0f1a` background and subtle radial glows
- Animated rotating conic-gradient border on the card and profile image
- Frosted glassmorphism card with backdrop blur and inner shadows
- Warm amber/gold accent palette (`#f59e0b`, `#d97706`, `#fbbf24`)
- Stats row displaying Projects, Followers, and Following counts
- Monochrome social icons with glow-on-hover effect
- Accent dots and divider lines on contact details
- Download CV and Contact call-to-action buttons
- Playfair Display serif font for the name, Inter for body text
- Uppercase letter-spaced role label
- Fully responsive for mobile and desktop

## Technical Requirements
- A modern web browser (Chrome, Edge, Safari recommended for full `@property` support)
- Internet connection for loading external libraries

## External Dependencies
- [Boxicons](https://boxicons.com/) — icons
- [Google Fonts](https://fonts.google.com/) — Inter and Playfair Display

## Installation

1. Clone the repository
```bash
git clone https://github.com/Hrk84ya/profile-card-project.git
```

2. Navigate to the project directory
```bash
cd profile-card-project
```

3. Open `index.html` in a web browser

4. (Optional) Customize the profile details by editing `index.html` and the CSS variables in `profile.css`

## Customization

### Color Scheme
All colors are controlled via CSS custom properties in `profile.css`:
```css
:root {
  --primary: #f59e0b;
  --secondary: #d97706;
  --accent: #fbbf24;
  --bg-dark: #0f0f1a;
  --bg-card: rgba(20, 20, 30, 0.7);
}
```
Change these values to switch the entire palette in one place.

### Contact Details
Update the `<li>` items inside the `.details` section in `index.html`:
```html
<li>
    <span class="accent-dot"></span>
    <i class="bx bx-envelope"></i>
    <span>your-email@example.com</span>
</li>
```

### Profile Image
Replace `img/Profile.jpg` with your own photo.

### Stats
Edit the numbers and labels in the `.stats-row` section of `index.html`.

## Browser Support
The animated gradient border uses the CSS `@property` rule, which is supported in Chrome, Edge, and Safari. Firefox will gracefully degrade to a static gradient.

## Contributing
Contributions are welcome!

1. Fork the repository
2. Create a new branch (`git checkout -b feature-name`)
3. Make your changes and commit (`git commit -m "Add feature or fix bug"`)
4. Push to the branch (`git push origin feature-name`)
5. Open a pull request

## Reporting Bugs or Issues
To report a bug, request a feature, or suggest improvements, please open an issue.
