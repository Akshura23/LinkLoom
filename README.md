# LinkLoom

LinkLoom is a static, browser-based QR generator. Add several links to create one QR code that opens a page with a button for each link.

## Deploy to Vercel

This project is plain HTML, CSS, and JavaScript. It has no build step, server, or environment variables.

1. Import this repository into Vercel.
2. Use the project root containing `index.html` and `vercel.json` as the Root Directory.
3. Deploy with the checked-in Vercel settings. The build command and install command are empty; the project root is served as static output.
4. Open the **production** deployment URL, enter your links, and generate the QR code you plan to share.

The QR points back to the exact host used when it was generated. Use your stable production URL or custom domain before printing or sharing it; preview deployment URLs may change.

## Local preview

Open `index.html` for a visual preview. QR codes that open the link page can only be generated from an HTTP(S) deployment, because a `file://` address is not reachable by other devices.

QR generation uses the QRCode.js library from cdnjs, so the generator needs an internet connection when it loads.
