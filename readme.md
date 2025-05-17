# Color Blindness Simulator

A modern, interactive web application that simulates various types of color blindness to help designers, developers, and educators create more accessible content. Built with vanilla JavaScript and featuring a sleek glassmorphism UI with dark/light mode toggle.

## 🌈 Features

- **Multiple Simulation Types**: Visualize 8 different types of color vision deficiency:
  - Protanopia (Red-Blind)
  - Protanomaly (Red-Weak)
  - Deuteranopia (Green-Blind)
  - Deuteranomaly (Green-Weak)
  - Tritanopia (Blue-Blind)
  - Tritanomaly (Blue-Weak)
  - Achromatopsia (Monochromacy)
  - Normal Vision (for comparison)

- **Image Upload**: Upload and process your own images to see how they appear to people with different types of color blindness

- **Color Comparison Grid**: Interactive comparison of common colors showing how they are perceived with different vision types

- **Educational Information**: Learn about each type of color blindness with detailed descriptions

- **Modern Glassmorphism UI**: Sleek, modern interface with frosted glass effect

- **Dark/Light Mode**: Toggle between dark and light themes based on your preference

## 🚀 Live Demo

[View the Live Demo](https://r3dhulk.github.io/color-blindness-simulator/)

## 📋 How It Works

The simulator uses color transformation matrices to convert standard RGB colors into their color-blind equivalent representations. These matrices mathematically simulate how colors are perceived by individuals with various types of color vision deficiency.

### Color Matrix Transformations

For each type of color blindness, a specific mathematical matrix is applied to transform RGB values:

```javascript
// Example: Deuteranopia transformation matrix
deuteranopia: [
    0.625, 0.375, 0, 0, 0,
    0.7, 0.3, 0, 0, 0,
    0, 0.3, 0.7, 0, 0,
    0, 0, 0, 1, 0
]
```

These matrices are derived from scientific research on color perception and provide accurate simulations of how colors appear to people with different types of color blindness.

## 💻 Installation & Usage

1. **Clone the repository**:
   ```bash
   git clone https://github.com/r3dhulk/color-blindness-simulator.git
   cd color-blindness-simulator
   ```

2. **Open in your browser**:
   - Simply open the `index.html` file in a modern web browser

3. **Using the simulator**:
   - Select a color blindness type from the dropdown
   - Upload an image to see how it appears with the selected condition
   - Explore the color grid to understand how specific colors appear
   - Toggle between dark and light themes as needed

## 🛠️ Technical Implementation

- **Pure JavaScript**: Built with vanilla JavaScript, no frameworks required
- **Canvas API**: Uses HTML5 Canvas for image processing and transformation
- **FileReader API**: Enables client-side image upload and processing
- **CSS Variables**: Dynamic theme switching with CSS custom properties

## 🔬 Understanding Color Blindness

Color vision deficiency affects approximately 1 in 12 men and 1 in 200 women worldwide. Understanding how your content appears to users with color blindness is crucial for creating accessible designs.

### Types of Color Blindness

- **Red-Green Color Blindness**: Most common, includes Protanopia, Protanomaly, Deuteranopia, and Deuteranomaly
- **Blue-Yellow Color Blindness**: Less common, includes Tritanopia and Tritanomaly
- **Complete Color Blindness**: Very rare, includes Achromatopsia (total color blindness)

## 🎨 Accessibility Tips

- **Don't rely solely on color** to convey information
- **Use patterns and textures** in addition to color
- **Maintain high contrast** ratios
- **Test your designs** with a simulator like this one
- **Use color-blind friendly palettes** when possible

## 📱 Responsive Design

The application is fully responsive and works on:
- Desktop computers
- Tablets
- Mobile devices

## 🧩 Future Improvements

- [ ] Add ability to download simulated images
- [ ] Implement URL image loading
- [ ] Create a color picker for custom color simulation
- [ ] Add browser extension version
- [ ] Implement webcam support for real-time simulation

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

Made with ❤️ for web accessibility