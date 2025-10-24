<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Link Reference</title>
    <!-- CSS is included directly here to make it a single, stylish file -->
    <style>
        /* Cosmic-Themed CSS for Links */
        body {
            background-color: #0c0d10; /* Dark background */
            color: #f0f0f0; 
            font-family: 'Lato', sans-serif;
            margin: 0;
            padding: 20px;
            line-height: 1.6;
        }

        .container {
            width: 90%;
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
            background: #1a1a38; /* Dark navy card background */
            border-radius: 12px;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.5);
        }

        h1 {
            color: #a29bfe; /* Light purple/blue accent */
            border-bottom: 2px solid #6c5ce7;
            padding-bottom: 10px;
            margin-top: 0;
        }

        h2 {
            color: #00cec9; /* Bright teal accent */
            margin-top: 30px;
        }

        /* Default link styling */
        a {
            color: #a29bfe; /* Default link color */
            text-decoration: none;
            transition: color 0.3s, border-bottom 0.3s;
            font-weight: bold;
        }

        /* Hover effect */
        a:hover {
            color: #00cec9; /* Bright teal on hover */
            border-bottom: 1px dashed #00cec9;
        }

        /* Button styling for links (Call to Action) */
        .cta-button {
            display: inline-block;
            background-color: #6c5ce7; 
            color: white !important; /* Override link color */
            padding: 12px 30px;
            text-decoration: none;
            border-radius: 5px;
            font-weight: bold;
            letter-spacing: 1px;
            margin: 10px 0;
            border: none;
        }

        .cta-button:hover {
            background-color: #a29bfe; 
            color: #0c0d10 !important;
            border-bottom: none;
        }

    </style>
</head>
<body>

    <div class="container">
        <h1>Essential HTML Link (Anchor Tag) `&lt;a&gt;` Guide</h1>
        <p>The `&lt;a&gt;` tag is used to create a hyperlink. The `href` attribute defines the destination.</p>

        <!-- 1. Linking to an External Website -->
        <h2>1. External Link (Opens in New Tab)</h2>
        <p>This links to another domain on the internet. Use `target="_blank"` to avoid navigating away from your own site.</p>
        <p>
            <a href="https://en.wikipedia.org/wiki/Black_hole" target="_blank">Read about Black Holes on Wikipedia &rarr;</a>
        </p>

        <!-- 2. Linking to Another Page on Your Site -->
        <h2>2. Internal Link (Local File)</h2>
        <p>This is how you link from your `index.html` to a blog post file (like `post-1.html`) within the same folder.</p>
        <p>
            <a href="post-1.html">Go to My First Blog Post (Post-1.html)</a>
        </p>

        <!-- 3. Linking to a Specific Section on the Same Page -->
        <h2>3. Link to Section on This Page (Anchor Link)</h2>
        <p>The link uses `#section-id` in the `href`. The destination section needs an `id` attribute.</p>
        <p>
            <a href="#jump-target">Jump to the Bottom Section of this Page</a>
        </p>

        <!-- 4. Link Styled as a Button -->
        <h2>4. Link Styled as a Call-to-Action Button</h2>
        <p>Perfect for featured posts or signing up for a newsletter.</p>
        <p>
            <a href="subscribe.html" class="cta-button">Subscribe to My Cosmic Insights</a>
        </p>

        <!-- 5. Link to Download a File -->
        <h2>5. Link to Download a PDF/File</h2>
        <p>Tells the browser to download the file instead of opening it.</p>
        <p>
            <a href="my_astrophysics_paper.pdf" download>Download My Research Paper (PDF)</a>
        </p>

        <!-- 6. Link to Send an Email -->
        <h2>6. Link to Send an Email</h2>
        <p>Opens the user's default email client.</p>
        <p>
            <a href="mailto:yourname@example.com?subject=Inquiry%20from%20Blog">Email the Author</a>
        </p>
        
        <br><br><br><br><br><br><br>
        
        <h2 id="jump-target">Destination Target</h2>
        <p>This is the section that the "Jump to the Bottom" link targets. Use this technique for Table of Contents links!</p>
        <p><a href="#">Back to Top</a></p>

    </div>

</body>
</html>
