<h1 align="center">
aRt</h1>

aRt is an R package to create generative art. Install using:
``` r
devtools::install_github("nrennie/aRt")
```
or
``` r
remotes::install_github("nrennie/aRt")
```

<h2 align="center">
attraction</h2>

The `attraction()` function produces generative art based on strange attractors.

``` r
attraction(n=50000, a=-3, b=1, c=0.5, d=-1, main_col="black", bg_col="white")
attraction(n=50000, a=-6, b=1, c=0.5, d=-2, main_col="black", bg_col="white")
attraction(n=50000, a=-3, b=-2, c=1, d=-1, main_col="SunsetDark", bg_col="white")
```
<p align="center">
<img src="/images/attraction1.jpeg?raw=true" width="30%">
<img src="/images/attraction2.jpeg?raw=true" width="30%">
<img src="/images/attraction3.jpeg?raw=true" width="30%">
</p>

<h2 align="center">
blending</h2>

The `blending()` function produces generative art of many boxes.

``` r
blending(n = 100, down = "white", up = "black", s = 1234)
blending(n = 500, down = "white", up = "black", s = 1234)
blending(n = 100, down = "#ba1141", up = "#003366", s = 1234)

```
<p align="center">
<img src="/images/blending1.jpeg?raw=true" width="30%">
<img src="/images/blending2.jpeg?raw=true" width="30%">
<img src="/images/blending3.jpeg?raw=true" width="30%">
</p>


<h2 align="center">
boxes</h2>

The `boxes()` function produces generative art of many boxes.

``` r
boxes(n=100, perc=0.1, col_palette="DarkMint", bg_col="black", s=1234)
boxes(n=20, perc=0.1, col_palette="DarkMint", bg_col="black", s=1234)
boxes(n=100, perc=0.5, col_palette="Magenta", bg_col="black", s=1234)
```
<p align="center">
<img src="/images/boxes_n100_p1.jpeg?raw=true" width="30%">
<img src="/images/boxes_n20_p1.jpeg?raw=true" width="30%">
<img src="/images/boxes_n100_p5.jpeg?raw=true" width="30%">
</p>

<h2 align="center">
bricks</h2>

The `bricks()` function draws multiple rectangular polygons in rows.

``` r
bricks(n_y=20, colours=c("#9B1D20", "#3D2B3D", "#CBEFB6", "#635D5C"), bg_col="gray97")
bricks(n_y=200, colours=c("#9B1D20", "#3D2B3D", "#CBEFB6", "#635D5C"), bg_col="gray97")
bricks(n_y=20, colours=carto_pal(7, "Burg"), bg_col="gray97")

```
<p align="center">
<img src="/images/bricks1.jpeg?raw=true" width="30%">
<img src="/images/bricks2.jpeg?raw=true" width="30%">
<img src="/images/bricks3.jpeg?raw=true" width="30%">
</p>


<h2 align="center">
bubbles</h2>

The `bubbles()` function produces generative art using layered polar bar charts.

``` r
bubbles(num_circles = 20, main_col = "black", col_palette = "Bold", bg_col = "white", s = 1234)
bubbles(num_circles = 20, main_col = "lightgrey", col_palette = "Bold", bg_col = "white", s = 123)
bubbles(num_circles = 10, main_col = "white", col_palette = "Prism", bg_col = "black", s = 2022)
```
<p align="center">
<img src="/images/bubbles1.jpeg?raw=true" width="30%">
<img src="/images/bubbles2.jpeg?raw=true" width="30%">
<img src="/images/bubbles3.jpeg?raw=true" width="30%">
</p>


<h2 align="center">
bullseye</h2>

The `bullseye()` function produces generative art using layered polar bar charts.

``` r
bullseye(main_col="black", bg_col="white", s=1234)
bullseye(main_col="white", bg_col="black", s=1234)
bullseye(main_col="black", bg_col="white", s=2021)
```
<p align="center">
<img src="/images/bullseye_1234.jpeg?raw=true" width="30%">
<img src="/images/bullseye_1234n.jpeg?raw=true" width="30%">
<img src="/images/bullseye_2021.jpeg?raw=true" width="30%">
</p>


<h2 align="center">
circles</h2>

The `circles()` function produces generative art using dendograms and circular graphs.

``` r
circles(n=100, smoothness=100, col_palette="Bold", line_col=NA, bg_col="black", s=1234)
circles(n=10, smoothness=100, col_palette="Bold", line_col=NA, bg_col="#e73f74", s=1234)
circles(n=2, smoothness=3, col_palette="Bold", line_col="black", bg_col="black", s=1234)
```
<p align="center">
<img src="/images/circles1.jpeg?raw=true" width="30%">
<img src="/images/circles2.jpeg?raw=true" width="30%">
<img src="/images/circles3.jpeg?raw=true" width="30%">
</p>

<h2 align="center">
circular</h2>

The `circular()` function produces circular generative art produced by many random paths from the centre of the circle.

``` r
circular(n=2, main_col="black", bg_col="white", s=56)
circular(n=10, main_col="black", bg_col="white", s=56)
circular(n=100, main_col="black", bg_col="white", s=56)
```
<p align="center">
<img src="/images/circular_n2.jpeg?raw=true" width="30%">
<img src="/images/circular_n10.jpeg?raw=true" width="30%">
<img src="/images/circular_n100.jpeg?raw=true" width="30%">
</p>

<h2 align="center">
connected</h2>

The `connected()` function produces generative art by connected points on a circle.

``` r
connected(n=100, n_geom=10, random=F, col_palette="RdPu", bg_col="#ae217e", s=1234)
connected(n=100, n_geom=10, random=T, col_palette="RdPu", bg_col="#ae217e", s=1234)
connected(n=250, n_geom=2, random=F, col_palette="RdPu", bg_col="#ae217e", s=1234)
```
<p align="center">
<img src="/images/connected_100_10F.jpeg?raw=true" width="30%">
<img src="/images/connected_100_10T.jpeg?raw=true" width="30%">
<img src="/images/connected_250_2F.jpeg?raw=true" width="30%">
</p>

<h2 align="center">
crawling</h2>

The `crawling()` function produces generative art using dendograms and tree graphs.

``` r
crawling(n=50, edge_colour="black", node_size=1, node_colour="black", bg_col="white", s=1234)
crawling(n=250, edge_colour="black", node_size=1, node_colour="black", bg_col="white", s=1234)
crawling(n=1000, edge_colour="black", node_size=1, node_colour="black", bg_col="white", s=1234)
```
<p align="center">
<img src="/images/crawling50.jpeg?raw=true" width="30%">
<img src="/images/crawling250.jpeg?raw=true" width="30%">
<img src="/images/crawling1000.jpeg?raw=true" width="30%">
</p>

<h2 align="center">
dots</h2>

The `dots()` function produces generative art using jittered points.

``` r
dots(n_x=50, n_y=100, jitter_size_width=0.5, jitter_size_height=0.5, col_palette = "Purp", bg_col="#63589f", s=1234)
dots(n_x=500, n_y=100, jitter_size_width=0.5, jitter_size_height=5, col_palette = "Purp", bg_col="#63589f", s=1234)
dots(n_x=50, n_y=100, jitter_size_width=0.05, jitter_size_height=50, col_palette = "Purp", bg_col="#63589f", s=1234)
```
<p align="center">
<img src="/images/dots1.jpeg?raw=true" width="30%">
<img src="/images/dots2.jpeg?raw=true" width="30%">
<img src="/images/dots3.jpeg?raw=true" width="30%">
</p>

<h2 align="center">
fading</h2>

The `fading()` function produces generative art using voronoi tiles.

``` r
fading(n_layers=6, n_points=10, col_palette="SunsetDark", s=1234)
fading(n_layers=6, n_points=1, col_palette="Sunset", s=1234)
fading(n_layers=10, n_points=10, col_palette="SunsetDark", s=1234)
```
<p align="center">
<img src="/images/fading_6_10.jpeg?raw=true" width="30%">
<img src="/images/fading_6_1.jpeg?raw=true" width="30%">
<img src="/images/fading_10_10.jpeg?raw=true" width="30%">
</p>

<h2 align="center">
flow fields</h2>

The `flow_fields()` function produces generative art using particle traces. These functions are inspired by a blog post by [Will Chase](https://www.williamrchase.com/post/flow-fields-12-months-of-art-september/). 

``` r
flow_fields(n = 10000, granualarity = 1000, x_freq = 1, y_freq = 1, alpha = 1, line_col = c("#edf8fb","#bfd3e6","#9ebcda","#8c96c6","#8c6bb1","#88419d","#6e016b"), bg_col = "lightgrey", s = 1234)
flow_fields(n = 10000, granualarity = 1000, x_freq = 1, y_freq = 1, alpha = 0.3, line_col = "black", bg_col = "white", s = 1234)
flow_fields(n = 10000, granualarity = 1000, x_freq = 3, y_freq = 0.2, alpha = 1, line_col = c("#edf8fb","#bfd3e6","#9ebcda","#8c96c6","#8c6bb1","#88419d","#6e016b"), bg_col = "lightgrey", s = 1234)
```
<p align="center">
<img src="/images/flow_fields1.jpeg?raw=true" width="30%">
<img src="/images/flow_fields2.jpeg?raw=true" width="30%">
<img src="/images/flow_fields3.jpeg?raw=true" width="30%">
</p>

<h2 align="center">
heart</h2>

The `heart()` function draws a heart from many overlapping lines.

``` r
heart(n=25, col_scheme="mono", bg_col="black", s=1234)
heart(n=100, col_scheme="mono", bg_col="black", s=1234)
heart(n=25, col_scheme="rainbow", bg_col="black", s=1234)
```
<p align="center">
<img src="/images/heart_n25_m.jpeg?raw=true" width="30%">
<img src="/images/heart_n100_m.jpeg?raw=true" width="30%">
<img src="/images/heart_n25_r.jpeg?raw=true" width="30%">
</p>

<h2 align="center">
infinity</h2>

The `infinity()` function draws an infinity symbol from many overlapping lines.

``` r
infinity(n=25, col_scheme="mono", bg_col="black", s=1234)
infinity(n=100, col_scheme="mono", bg_col="black", s=1234)
infinity(n=25, col_scheme="rainbow", bg_col="black", s=1234)
```
<p align="center">
<img src="/images/infinity_n25_m.jpeg?raw=true" width="30%">
<img src="/images/infinity_n100_m.jpeg?raw=true" width="30%">
<img src="/images/infinity_n25_r.jpeg?raw=true" width="30%">
</p>

<h2 align="center">
polygons</h2>

The `polygons()` function draws multiple polygons.

``` r
polygons(n_x=12, n_y=18, gap_size=0.5, deg_jitter=0.1, colours=c("#9B1D20", "#3D2B3D", "#CBEFB6", "#635D5C"), rand = FALSE, bg_col="gray97")
polygons(n_x=6, n_y=9, gap_size=0.2, deg_jitter=0.1, colours=c("#9B1D20", "#3D2B3D", "#CBEFB6", "#635D5C"), rand = FALSE, bg_col="gray97")
polygons(n_x=12, n_y=18, gap_size=0.5, deg_jitter=0.5, colours=carto_pal(7, "Burg"), rand = FALSE, bg_col="gray97")

```
<p align="center">
<img src="/images/polygons1.jpeg?raw=true" width="30%">
<img src="/images/polygons2.jpeg?raw=true" width="30%">
<img src="/images/polygons3.jpeg?raw=true" width="30%">
</p>

<h2 align="center">
rectangles</h2>

The `rectangles()` function draws multiple rectangles.

``` r
rectangles(n = 100, max_height = 7, max_width = 5, size = 2, main_col = "lightgrey", col_palette = "Bold", bg_col = "white", s = 123)
rectangles(n = 10, max_height = 15, max_width = 15, size = 4, main_col = "lightgrey", col_palette = "Bold", bg_col = "white", s = 123)
rectangles(n = 100, max_height = 4, max_width = 6, size = 1, main_col = ggplot2::alpha("white", 0.5), col_palette = "Prism", bg_col = "black", s = 123)

```
<p align="center">
<img src="/images/rectangles1.jpeg?raw=true" width="30%">
<img src="/images/rectangles2.jpeg?raw=true" width="30%">
<img src="/images/rectangles3.jpeg?raw=true" width="30%">
</p>


<h2 align="center">
shell</h2>

The `shells()` function produces generative art using sine and cosine waves.

``` r
shells(n = 4, alpha = 1, main_col = "black", bg_col = "white")
shells(n = 10, alpha = 1, main_col = "black", bg_col = "white")
shells(n = 6, alpha = 0.5, main_col = "#CC338B", bg_col = alpha("#CC338B", 0.2))
```
<p align="center">
<img src="/images/shell1.jpeg?raw=true" width="30%">
<img src="/images/shell2.jpeg?raw=true" width="30%">
<img src="/images/shell3.jpeg?raw=true" width="30%">
</p>


<h2 align="center">
spirals</h2>

The `spirals()` function produces generative art consisting of dots arranged in a spiral.

``` r
spirals(perc=0.2, s=1234)
spirals(perc=0.5, s=1234)
spirals(perc=0.8, s=1234)
```
<p align="center">
<img src="/images/spirals_p2.jpeg?raw=true" width="30%">
<img src="/images/spirals_p5.jpeg?raw=true" width="30%">
<img src="/images/spirals_p8.jpeg?raw=true" width="30%">
</p>

<h2 align="center">
static</h2>

The `static()` function produces generative art reminiscent of the noise displayed on analog televisions when no transmission signal is received.

``` r
static(perc=0.01, n=500, s=1234)
static(perc=0.1, n=500, s=1234)
static(perc=0.3, n=500, s=1234)
```
<p align="center">
<img src="/images/static_p01_n500.jpeg?raw=true" width="30%">
<img src="/images/static_p10_n500.jpeg?raw=true" width="30%">
<img src="/images/static_p30_n500.jpeg?raw=true" width="30%">
</p>


<h2 align="center">
stripes</h2>

The `stripes()` function produces generative art consisting of rows of vertical stripes.

``` r
stripes(perc=0, n=3, col_palette = "TealGrn", alpha = 1, s=1234)
stripes(perc=0.5, n=3, col_palette = "TealGrn", alpha = 1, s=1234)
stripes(perc=1, n=3, col_palette = "TealGrn", alpha = 1, s=1234)
```
<p align="center">
<img src="/images/stripes_p00_n3.jpeg?raw=true" width="30%">
<img src="/images/stripes_p50_n3.jpeg?raw=true" width="30%">
<img src="/images/stripes_p100_n3.jpeg?raw=true" width="30%">
</p>

<h2 align="center">
tiles</h2>

The `tiles()` function produces generative art using square polygons.

``` r
tiles(n_x=12, n_y=12, col_palette="Veronese", num_colours=5, s=1234)
tiles(n_x=50, n_y=50, col_palette="Veronese", num_colours=6, s=1234)
tiles(n_x=12, n_y=12, col_palette="Pissaro", num_colours=5, s=1234)
```
<p align="center">
<img src="/images/tiles_veronese1.jpeg?raw=true" width="30%">
<img src="/images/tiles_veronese2.jpeg?raw=true" width="30%">
<img src="/images/tiles_pissaro1.jpeg?raw=true" width="30%">
</p>


<h2 align="center">
vortex</h2>

The `vortex()` function produces circular vortex generative art produced by a line plot and polar coordinates.

``` r
vortex(n=25, start_val=90, col_scheme="mono", bg_col="black", s=1234)
vortex(n=100, start_val=90, col_scheme="mono", bg_col="black", s=1234)
vortex(n=25, start_val=90, col_scheme="rainbow", bg_col="black", s=1234)
```
<p align="center">
<img src="/images/vortex_n25_m.jpeg?raw=true" width="30%">
<img src="/images/vortex_n100_m.jpeg?raw=true" width="30%">
<img src="/images/vortex_n25_r.jpeg?raw=true" width="30%">
</p>


<h2 align="center">
waves</h2>

The `waves()` function produces generative art using sine and cosine waves.

``` r
waves(a=23, b=6, main_col="white", bg_col="black", s=2021)
waves(a=23, b=6, main_col="Prism", bg_col="#edad08", s=2021)
waves(a=6, b=23, main_col="black", bg_col="white", s=2021)
```
<p align="center">
<img src="/images/waves23_6_bw.jpeg?raw=true" width="30%">
<img src="/images/waves23_6_col.jpeg?raw=true" width="30%">
<img src="/images/waves6_23_bw.jpeg?raw=true" width="30%">
</p>

