---
layout: default
title: Home
permalink: /
---

<div style="position: relative; width: 100%; height: 60vh; overflow: hidden;">
  <img src="https://juliocedillo.github.io/neweconomy/assets/images/pediment.png" alt="header" style="width: 100%; height: 100%; object-fit: cover; border: none;">
  <div style="position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); color: white; font-size: 24px; font-weight: bold; text-align: center; max-width: 80%; line-height: 1.4;">
    如果过去40年经济历史中所遵循的规则只是一次性的、具有历史偶然性的产物，而这些规则如今正迅速走向终结，会怎样呢？
  </div>
</div>

<p>&nbsp;&nbsp;&nbsp;</p>

阿曼多·拉拉-米兰（Armando Lara-Millan）正在撰写一本暂定名为《预见未来的公司与新全球经济的诞生》的书。书中论证，在过去四十年里，全球经济中的五大政治经济动态被广泛误认为是全球化经济的新、永久规则。实际上，它们不过是一次性的、具有历史偶然性的变革，如今正迅速发生变化。

拉拉-米兰结合对一家关键投资公司的定性研究以及对数十年企业季度报告的自然语言处理，详细描述了中国低成本劳动力的终结、高增长向周期性互联网受益行业的转变、廉价能源向昂贵原材料的过渡、企业税收和借贷成本无法进一步降低，以及表演性货币政策的不确定作用。本书为理解所谓的“多重危机”提供了一种新的视角，帮助更好地认识当前正处于挣扎诞生中的新秩序。
<p>&nbsp;&nbsp;&nbsp;</p>

---

|目标 |方法|作用|
|---|---|---|
|我们的项目调查了中国低成本劳动力的终结和硅谷宽松货币环境的消退，探索旧油田和煤田中的铜和锂矿藏，以及杰克逊霍尔和欧洲央行官员们的语言博弈。通过结合对关键资产管理公司的民族志研究、对全球重点行业雇主和员工的访谈，以及对数十年主要企业季度报告的自然语言处理，“全球经济的未来”项目致力于理解新全球秩序如何在当下艰难诞生。|通过编织对关键资产管理公司的民族志研究、对全球重点行业雇主和员工的访谈，以及对各大公司数十年季度报告的自然语言处理，“全球经济的未来”项目致力于理解新全球秩序如何在当下艰难诞生。|将过去40年置于历史脉络中，我们将关于“新自由主义”、“金融化”和“超全球化”等不同论点编织在一起。通过这样做，我们希望理清当代的“多重危机”，并理解一个新的全球秩序如何在当下艰难诞生。|
---

<p>&nbsp;&nbsp;&nbsp;</p>

<h1 style="text-align: center;">我们所研究的动态</h1>

<!-- HTML for the Carousel -->
<div class="carousel">
  <div class="carousel-container">
    <img class="carousel-slide" src="https://juliocedillo.github.io/neweconomy/assets/images/q3_zh.png" alt="Image 1">
    <img class="carousel-slide" src="https://juliocedillo.github.io/neweconomy/assets/images/q2_zh.png" alt="Image 2">
    <img class="carousel-slide" src="https://juliocedillo.github.io/neweconomy/assets/images/q1_zh.png" alt="Image 3">
    <img class="carousel-slide" src="https://juliocedillo.github.io/neweconomy/assets/images/q4_zh.png" alt="Image 4">
    <img class="carousel-slide" src="https://juliocedillo.github.io/neweconomy/assets/images/q5_zh.png" alt="Image 5">
  </div>
  <button class="carousel-prev" onclick="moveSlide(-1)">&#10094;</button>
  <button class="carousel-next" onclick="moveSlide(1)">&#10095;</button>
</div>

<!-- CSS for styling the Carousel -->
<style>
  .carousel {
  position: relative;
  max-width: 800px;
  margin: auto;
  overflow: hidden;
  }

  .carousel-container {
    display: flex;
    transition: transform 0.5s ease;
  }

  .carousel-slide {
    width: 800px;
    flex-shrink: 0;
    display: block;
  }

  .carousel-prev, .carousel-next {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    background-color: rgba(0, 0, 0, 0.5);
    color: white;
    border: none;
    padding: 16px;
    cursor: pointer;
    z-index: 10;
  }

  .carousel-prev {
    left: 0;
  }

  .carousel-next {
    right: 0;
  }
</style>

<script>
  let currentIndex = 0;

  function moveSlide(direction) {
    const slides = document.querySelectorAll('.carousel-slide');
    const totalSlides = slides.length;

    currentIndex = (currentIndex + direction + totalSlides) % totalSlides;

    updateSlidePosition();
  }

  function updateSlidePosition() {
    const slides = document.querySelectorAll('.carousel-slide');
    if (slides.length === 0) return;
    const slideWidth = slides[0].offsetWidth;
    document.querySelector('.carousel-container').style.transform =
      `translateX(-${currentIndex * slideWidth}px)`;
  }

  // Ensure layout is calculated before applying transform
  window.addEventListener('DOMContentLoaded', () => {
    setTimeout(updateSlidePosition, 100);
  });
</script>
