+++
title = 'Adoptieren'
date = 2025-05-24
+++
**1**
{{< figure src="static/images/strays-in-need-serbia.svg" alt="Mein Bild" width="300px" >}}
**2**
{{ $img := "static/strays-in-need-serbia.jpg" | relURL }}
<img src="{{ $img }}" alt="Mein Bild" width="300px">

**3**
{{ $img := "/static/strays-in-need-serbia.jpg" | absURL }}
<img src="{{ $img }}" alt="Mein Bild" width="300px">