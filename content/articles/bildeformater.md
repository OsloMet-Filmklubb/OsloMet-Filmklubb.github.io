---
draft: false
title: "Bildeformater"
# summary: ""
cover: ""
---
<div class="grid">

<div>

# Movietone
{{< aspect-ratio 1.19 >}}
</div>

<div>

# Stumfilm 4:3
{{< aspect-ratio 1.33 >}}
</div>
<div>

# Academy Ratio
{{< aspect-ratio 1.375 >}}
</div>
<div>

# 70mm IMAX
{{< aspect-ratio 1.43 >}}
</div>
<div>

# HDTV 16:9
{{< aspect-ratio 1.78 >}}
</div>
<div>

# Flat
{{< aspect-ratio 1.85 >}}
</div>
<div>

# 70mm
{{< aspect-ratio 2.20 >}}
</div>
<div>

# Scope
{{< aspect-ratio 2.39 >}}
</div>
</div>

<style>
    .grid{
        display: grid;
        column-gap: 4%;
        grid-template-columns: 48% 48%;
    }

    .grid > * {
        font-size: 30px;
        text-align: center;
    }

    @media (max-width: 684px) {
        .grid{
            grid-template-columns: 100%;
        }
        .grid > * {
            text-align: start;
        }
    }
</style>