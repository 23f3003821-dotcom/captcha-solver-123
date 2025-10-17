# Captcha Solver Frontend

This is a simple, single-file responsive HTML application designed to act as a frontend for solving CAPTCHAs. It utilizes Tailwind CSS for styling and responsiveness.

## Features

*   **Dynamic Image Loading:** Displays a CAPTCHA image, defaulting to `sample.png` if no specific image URL is provided.
*   **URL Parameter Support:** Can load a CAPTCHA image from a URL specified in the query string (e.g., `index.html?url=https://example.com/captcha.png`).
*   **User Input Field:** Provides an input field for users to type the CAPTCHA text.
*   **Basic Client-Side Verification (for `sample.png`):** Includes a rudimentary client-side check for the default `sample.png` image (expected text: "ADCRB"). *Note: For actual CAPTCHA solving, a robust backend or advanced client-side libraries would be required.*
*   **Responsive Design:** Adapts to various screen sizes using Tailwind CSS.

## How to Use

1.  **Open `index.html`:** Simply open the `index.html` file in your web browser.
2.  **Default CAPTCHA:** By default, the application will display `sample.png`.
3.  **Custom CAPTCHA URL:** To display a different CAPTCHA image, append the `url` query parameter to the URL in your browser's address bar.
    *   Example: `index.html?url=https://your-domain.com/path/to/your/captcha.png`
4.  **Enter CAPTCHA:** Type the text you see in the image into the input field.
5.  **Verify:** Click the "Verify Captcha" button or press Enter.

## Development

This application is built with:

*   **HTML5:** For structure.
*   **Tailwind CSS (CDN):** For styling and responsiveness.
*   **Vanilla JavaScript:** For dynamic content and interaction.

## Project Structure

*   `index.html`: The main single-file HTML application.
*   `README.md`: This file.
*   `LICENSE`: The MIT License for this project.
*   `sample.png`: The default CAPTCHA image.

## Limitations

*   **Client-Side Verification:** The built-in verification is very basic and only works for the `sample.png` file with a hardcoded value. A real CAPTCHA system requires server-side validation.
*   **Automatic Solver:** This application does *not* automatically solve CAPTCHAs. It provides a user interface for manual input.
*   **CORS:** If you try to load external CAPTCHA images, Cross-Origin Resource Sharing (CORS) policies of the image's host server might prevent the image from loading directly if it's served from a different domain without appropriate headers.

---

Feel free to adapt and extend this project for more advanced CAPTCHA integration!