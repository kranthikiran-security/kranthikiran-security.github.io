---
layout: post
title:  Embed PDF in HTML Page
categories: [HTML,Code]
---

This post demonstrate how to embed a Non downloadable PDF File in the HTML webpage.

This is the code snippet:

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
Example given below

```
/uploads/resume.pdf

```
