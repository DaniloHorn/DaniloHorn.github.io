+++
title = 'Adoptieren'
date = 2025-05-24
+++
**1**
{{< figure src="/images/strays-in-need-serbia.jpg" alt="Mein Bild" width="300px" >}}
**2**
{{ $img := "/images/strays-in-need-serbia.jpg" | relURL }}
<img src="{{ $img }}" alt="Mein Bild" width="300px">
**3**
{{ $img := "/images/strays-in-need-serbia.jpg" | absURL }}
<img src="{{ $img }}" alt="Mein Bild" width="300px">