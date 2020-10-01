<!-- define the wrapper and the container -->
    <div data-barba="wrapper">
      <div data-barba="container" data-barba-namespace="page-a">
        <h1>Home</h1>
      </div>
    </div>

    <!-- load barba (UMD version) -->
    <script src="https://unpkg.com/@barba/core"></script>

    <!-- load gsap animation library (minified version) -->
    <script src="https://unpkg.com/gsap@latest/dist/gsap.min.js"></script>

    <!-- init barba with a simple opacity transition -->
    <script type="text/javascript">
      barba.init({
        transitions: [{
          name: 'opacity-transition',
          leave(data) {
            return gsap.to(data.current.container, {
              opacity: 0
            });
          },
          enter(data) {
            return gsap.from(data.next.container, {
              opacity: 0
            });
          }
        }]
      });
    </script>


<script type="text/javascript" charset="utf-8" 
src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML,
https://vincenttam.github.io/javascripts/MathJaxLocal.js"></script>

$$
x_{1,2} = \frac{-5 \pm \sqrt{5^2-12}}{6}
$$

![visitors](https://visitor-badge.glitch.me/badge?page_id=rangavirender.site.others)

<p align="center">
<img src="logo_v1.png" width="30">
</p>
