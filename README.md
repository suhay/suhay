<!-- ![](https://suhay.github.io/suhay/images/mug.svg) -->

<svg viewBox="0 0 904 400" width="904px" height="400px" xmlns="http://www.w3.org/2000/svg" xmlns:bx="https://boxy-svg.com">
  <style type="text/css">
    #test { display: none; }
  </style>
  <defs>
    <linearGradient id="base" bx:pinned="true">
      <stop style="stop-color: rgb(255, 255, 255);"/>
    </linearGradient>
    <filter id="drop-shadow-filter-1" x="-500%" y="-500%" width="1000%" height="1000%" bx:pinned="true">
      <title>outter</title>
      <feFlood x="10" y="10" result="flood-0" style="flood-color: rgb(242, 238, 255); flood-opacity: 0.48;"/>
      <feGaussianBlur in="SourceAlpha" stdDeviation="10" result="gaussian-blur-0"/>
      <feOffset dx="-4" dy="-4" in="gaussian-blur-0" result="offset-0"/>
      <feComponentTransfer result="offsetblur" in="offset-0">
        <feFuncA id="spread-ctrl" type="linear" slope="2"/>
      </feComponentTransfer>
      <feComposite in2="offsetblur" operator="in" in="flood-0" result="composite-0"/>
      <feMerge result="merge-0">
        <feMergeNode in="composite-0"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
      <feFlood x="10" y="10" result="flood-1" style="flood-opacity: 0.1;"/>
      <feOffset dx="6" dy="6" in="gaussian-blur-0" result="offset-1"/>
      <feComponentTransfer result="component-transfer-0" in="offset-1">
        <feFuncA id="spread-ctrl" type="linear" slope="2"/>
      </feComponentTransfer>
      <feComposite in2="component-transfer-0" operator="in" in="flood-1" result="composite-1"/>
      <feMerge result="merge-2">
        <feMergeNode in="composite-1"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
      <feMerge result="merge-1">
        <feMergeNode in="merge-0"/>
        <feMergeNode in="merge-2"/>
      </feMerge>
    </filter>
    <filter id="inner-shadow-filter-0" x="-500%" y="-500%" width="1000%" height="1000%">
      <title>inner dark</title>
      <feOffset dx="1" dy="10" in="SourceGraphic" result="offset-0"/>
      <feGaussianBlur stdDeviation="4" in="offset-0" result="gaussian-blur-0"/>
      <feComposite operator="out" in="SourceGraphic" result="composite-0" in2="gaussian-blur-0"/>
      <feComponentTransfer result="choke" in="composite-0">
        <feFuncA type="linear" slope="0.36"/>
      </feComponentTransfer>
      <feFlood flood-color="rgba(0,0,0,0.74)" result="color"/>
      <feComposite operator="in" in="color" in2="choke" result="shadow"/>
      <feComposite operator="over" in="shadow" in2="SourceGraphic" result="composite-1"/>
    </filter>
    <filter id="filter-1" x="-500%" y="-500%" width="1000%" height="1000%">
      <title>inner light</title>
      <feOffset dx="-3" dy="-3" in="SourceGraphic" result="offset-0"/>
      <feGaussianBlur stdDeviation="11" in="offset-0" result="gaussian-blur-0"/>
      <feComposite operator="out" in="SourceGraphic" result="composite-0" in2="gaussian-blur-0"/>
      <feComponentTransfer result="choke" in="composite-0">
        <feFuncA type="linear" slope="0.96"/>
      </feComponentTransfer>
      <feFlood flood-color="rgba(242,238,255,1)" result="color"/>
      <feComposite operator="in" in="color" in2="choke" result="shadow"/>
      <feComposite operator="over" in="shadow" in2="SourceGraphic" result="composite-1"/>
    </filter>
  </defs>
  <g style="filter: none;" transform="matrix(1, 0, 0, 1, -32.483162, -4.997409)">
    <path style="fill: url(#base); filter: url(#drop-shadow-filter-1);" d="M 571.294 94.628 C 571.36 79.265 649.341 72.756 687.182 73.997 C 720.923 75.103 781.879 78.333 796.892 94.393 C 801.244 99.049 797.351 125.008 799.119 124.917 C 819.366 123.874 844.01 115.678 859.895 122.587 C 881.856 132.14 891.147 146.383 894.667 170.072 C 898.834 198.12 883.712 231.333 863.024 251.479 C 838.351 275.505 788.944 318.259 762.277 322.144 C 759.467 322.553 756.162 338.392 748.543 343.443 C 729.45 356.1 696.874 355.442 685.57 355.698 C 677.096 355.89 636.322 357.26 619.483 343.592 C 614.309 339.392 615.673 335.631 612.507 331.211 C 597.665 310.49 588.079 286.298 581.862 260.592 C 568.98 207.324 571.113 136.892 571.294 94.628 Z">
      <title>cup</title>
    </path>
    <path style="fill: url(#base); filter: url(#filter-1);" d="M 785.552 273.355 C 790.063 251.524 798.161 198.902 796.164 184.706 C 795.567 180.46 805.028 178.312 806.233 175.032 C 818.407 141.878 829.037 139.296 845.533 138.714 C 866.146 137.987 877.762 164.261 878.55 182.979 C 879.722 210.812 843.876 247.515 819.745 265.338 C 805.478 275.875 784.27 279.557 785.552 273.355 Z">
      <title>handle - light</title>
    </path>
    <path style="fill: url(#base); filter: url(#inner-shadow-filter-0); opacity: 0.5;" d="M 785.552 273.355 C 790.063 251.524 798.161 198.902 796.164 184.706 C 795.567 180.46 805.028 178.312 806.233 175.032 C 818.407 141.878 829.037 139.296 845.533 138.714 C 866.146 137.987 877.762 164.261 878.55 182.979 C 879.722 210.812 843.876 247.515 819.745 265.338 C 805.478 275.875 784.27 279.557 785.552 273.355 Z">
      <title>handle - dark</title>
    </path>
    <path style="fill: url(#base); filter: url(#filter-1); paint-order: stroke;" d="M 790.179 97.557 C 790.943 82.038 718.522 77.935 683.405 77.248 C 646.496 76.526 578.461 82.548 578.237 94.34 C 577.943 109.831 688.23 113.242 688.23 113.242 C 688.23 113.242 789.54 110.531 790.179 97.557 Z">
      <title>rim - light</title>
    </path>
    <path style="filter: url(#inner-shadow-filter-0); paint-order: fill markers; fill: url(#base); opacity: 0.29;" d="M 790.179 97.557 C 790.943 82.038 718.522 77.935 683.405 77.248 C 646.496 76.526 578.461 82.548 578.237 94.34 C 577.943 109.831 688.23 113.242 688.23 113.242 C 688.23 113.242 789.54 110.531 790.179 97.557 Z">
      <title>rim - dark</title>
    </path>
  </g>
</svg>

<style type="text/css">
  #test2 { display: none; }
</style>

<!--
**suhay/suhay** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
