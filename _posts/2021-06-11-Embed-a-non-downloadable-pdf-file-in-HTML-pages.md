---
layout: post
title:  Embed PDF in HTML Page
categories: [HTML,Code]
---

This post demonstrate how to embed a PDF File in the HTML webpage.

This code snippet below helps how to add the Simple PDF File using <iframe> tag.
```
<!DOCTYPE html>
<html>
  <head>
    <title>Title of the document</title>
  </head>
  <body>
    <h1>PDF Example with iframe</h1>   
    <iframe src="link/to/your.pdf" width="100%" height="500px">
    </iframe>
  </body>
</html>

```

This is the code snippet for embedding Non downloadable PDF File:
```
<!DOCTYPE html>
<html>
  <head>
    <title>Title of the document</title>
  </head>
  <body>
    <h1>How to disable downloading of the PDF document</h1>
    <iframe src="/yourpdfLocation.pdf#toolbar=0" width="100%" height="500px">
    </iframe>
  </body>
</html>

```

Replace the above yourpdfLocation with Path of the PDF File.
Example path given below:
```
/uploads/resume.pdf

```
