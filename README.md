# LinkLoom

LinkLoom is a static, browser-based QR generator. Enter one URL to create one QR code that opens that URL directly. Optionally add a logo to the center of the code.

## Deploy to Vercel

This project is plain HTML, CSS, and JavaScript. It has no build step, server, or environment variables.

1. Import this repository into Vercel.
2. Use the project root containing `index.html` and `vercel.json` as the Root Directory.
3. Deploy with the checked-in Vercel settings. The build command and install command are empty; the project root is served as static output.
4. Open the **production** deployment URL, enter your links, and generate the QR code you plan to share.

The destination URL is encoded directly into the QR. The optional logo is composited in your browser and is not uploaded.

## Local preview

Open `index.html` for a visual preview. QR generation and logo processing happen in your browser.

QR generation uses the QRCode.js library from cdnjs, so the generator needs an internet connection when it loads.
