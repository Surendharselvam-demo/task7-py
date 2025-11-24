A simple and user-friendly Image Resizer Tool built using HTML, CSS, and JavaScript.
This tool allows users to upload an image, enter custom dimensions, preview the resized image, and download it instantly.

🚀 Features

📤 Upload any image (JPG, PNG, WEBP, etc.)

✏️ Enter custom width and height

🔍 Live preview of the resized image

📥 Download resized output as PNG

🎨 Clean and responsive UI

⚡ No backend required — runs completely in browser

🛠️ Technologies Used

HTML5

CSS3

JavaScript (Canvas API)

📂 Project Structure
image-resizer/
│── index.html
│── README.md

▶️ How to Use

Open the index.html file in any modern browser.

Click Choose File to upload an image.

Enter the new width and height (in pixels).

Click Resize Image.

Preview will update instantly.

Click Download Resized Image to save it.

📌 How It Works
1️⃣ Load image

The selected image is read using:

const reader = new FileReader();
reader.readAsDataURL(file);

2️⃣ Draw on Canvas

The image is resized using an HTML <canvas>:

ctx.drawImage(img, 0, 0, width, height);

3️⃣ Convert to image

Canvas output is converted to a PNG:

const resizedURL = canvas.toDataURL("image/png");
