<!DOCTYPE html>
<html lang="en">
<head>
<link href="fonts.googleapis.com" rel="stylesheet">

<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Text-To-PDF</title>
<meta name="description" content="Convert text and LaTeX math formulas into PDF online using ChatGPT, Copilot, and Google AI. Fast, free, and easy to use.">
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/katex@0.16.8/dist/katex.min.css">
<script defer src="https://cdn.jsdelivr.net/npm/katex@0.16.8/dist/katex.min.js"></script>
<script defer src="https://cdn.jsdelivr.net/npm/katex@0.16.8/dist/contrib/auto-render.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/html2canvas/1.4.1/html2canvas.min.js"></script>

<style>
body { font-family: Arial; background: #eef7ff; margin:0; padding:0; }
.navbar { display:flex; justify-content:space-between; align-items:center; background:#6bb6ff; color:white; padding:10px 20px; }
.nav-links { list-style:none; display:flex; gap:15px; margin:0; padding:0; }
.nav-links li a { color:white; text-decoration:none; font-weight:bold; }
.container { padding:20px; max-width:900px; margin:auto; }
.input-box { width:100%; min-height:200px; padding:15px; border:2px solid #6bb6ff; border-radius:10px; background:white; font-size:18px; outline:none; }
.preview { width:100%; min-height:200px; margin-top:20px; padding:15px; border:2px solid #6bb6ff; border-radius:10px; background:white; }
.btn-box { margin-top:20px; display:flex; gap:10px; }
button { padding:10px 15px; border:none; border-radius:5px; background:#6bb6ff; color:white; cursor:pointer; }
button:hover { background:#559fd6; }
footer { text-align:center; padding:10px; margin-top:20px; background:#6bb6ff; color:white; }
.seo-section { margin-top:30px; background:white; padding:20px; border-radius:10px; border:2px solid #6bb6ff; }
.seo-section h2 { margin-top:0; }
</style>
</head>
<body>

<nav class="navbar">
<div class="logo" id="Websitename">My PDF</div>
<ul class="nav-links">
<li><a href="#">Home</a></li>
<li><a href="#">Convert</a></li>
<li><a href="#">Tools</a></li>
<li><a href="#contact">Contact</a></li>

</ul>
</nav>

<div class="container">
<h1>ChatGPT, Copilot and Google AI can convert text into PDF Online</h1>
<div id="inputBox" contenteditable="true" class="input-box">
Paste Text Here............
</div>
<div class="btn-box">
<button onclick="downloadPDF()">Download PDF</button>
<button onclick="clearText()">Clear</button>
</div>



<!-- SEO-Friendly Content Section -->
<section class="seo-section">
<h2>Convert Text and Math Formulas to PDF Easily</h2>
<p>Our online tool uses advanced AI like <strong>ChatGPT, Copilot, and Google AI</strong> to convert your text and LaTeX math formulas into professional PDF documents. It preserves all formatting, symbols, and equations for accurate output.</p>

<h3>Features:</h3>
<ul>
<li>Instantly convert text and math formulas to PDF.</li>
<li>Supports LaTeX equations and special symbols.</li>
<li>High-quality PDF output suitable for printing and sharing.</li>
<li>User-friendly interface, no installation needed.</li>
<li>Free and accessible on any device or browser.</li>
</ul>

<h3>How to Use:</h3>
<ol>
<li>Type or paste your text and formulas into the input box above.</li>
<li>Click "Preview" to see your formatted content or "Download PDF" to generate the PDF.</li>
<li>Save or share your PDF instantly. Formatting and equations remain intact.</li>
</ol>

<p>This tool is ideal for students, teachers, researchers, and professionals who need accurate PDF conversion for text and mathematical content.</p>
</section>

</div>


<footer>© 2025 | My PDF Tools | All Rights Reserved | <a href="https://wa.me/9423650076" target="_blank" class="whatsapp-btn">
  <img src="https://upload.wikimedia.org/wikipedia/commons/6/6b/WhatsApp.svg" 
       alt="WhatsApp" width="24" style="vertical-align:middle; margin-right:8px;">
       
</footer>

<script>
function renderMath(element) {
    renderMathInElement(element, {
        delimiters: [
            {left: "\\[", right: "\\]", display: true},
            {left: "$$", right: "$$", display: true},
            {left: "\\(", right: "\\)", display: false},
            {left: "$", right: "$", display: false}
        ]
    });
}

function previewContent() {
	const input = document.getElementById("inputBox").innerHTML;
    const preview = document.getElementById("preview");
    preview.innerHTML = input;
    renderMath(preview);
}

function clearText() {
    document.getElementById("inputBox").innerText = "";
    document.getElementById("preview").innerHTML = "";
}

async function downloadPDF() {
    previewContent(); // update preview first
    const preview = document.getElementById("inputBox");
    preview.style.background = "#ffffff";

    await new Promise(r => setTimeout(r, 200)); // wait KaTeX render

    const scale = 2;
    const canvas = await html2canvas(preview, { scale: scale, useCORS:true, backgroundColor:"#ffffff" });

    const { jsPDF } = window.jspdf;
    const pdf = new jsPDF('p', 'px', 'a4');
    const pdfWidth = pdf.internal.pageSize.getWidth();
    const pdfHeight = pdf.internal.pageSize.getHeight();
    const imgWidth = pdfWidth;
    const imgHeight = (canvas.height * pdfWidth) / canvas.width;

    if(imgHeight <= pdfHeight){
        const imgData = canvas.toDataURL('image/png');
        pdf.addImage(imgData, 'PNG', 0,0, imgWidth, imgHeight);
        pdf.save("pavanja.pdf");
    } else {
        let remainingHeight = canvas.height;
        let positionY = 0;
        const sliceHeightPx = Math.floor((pdfHeight * canvas.width) / pdfWidth);

        while(remainingHeight > 0){
            const actualSliceHeight = Math.min(sliceHeightPx, remainingHeight);
            const tmpCanvas = document.createElement('canvas');
            tmpCanvas.width = canvas.width;
            tmpCanvas.height = actualSliceHeight;
            const ctx = tmpCanvas.getContext('2d');
            ctx.drawImage(canvas, 0, positionY, canvas.width, actualSliceHeight, 0,0, canvas.width, actualSliceHeight);

            const imgData = tmpCanvas.toDataURL('image/png');
            const renderHeight = (actualSliceHeight * pdfWidth) / canvas.width;
            pdf.addImage(imgData, 'PNG', 0,0, imgWidth, renderHeight);

            remainingHeight -= actualSliceHeight;
            positionY += actualSliceHeight;

            if(remainingHeight > 0) pdf.addPage();
        }
        pdf.save("My PDF.pdf");
    }
}
</script>

</body>
</html>
