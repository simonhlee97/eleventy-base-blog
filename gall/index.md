---
layout: layouts/gallery.njk
title: Gallery
templateClass: tmpl-post
eleventyNavigation:
  key: Gallery
  order: 4
---
<style>
    * {
      box-sizing: border-box;
    }

    /* body {
      padding: 50px;
      font-family: "Avenir", sans-serif;
      background: linear-gradient(to right, #F33D33, #6D3733);
    } */

    .close {
      background: none;
      color: white;
      border: 0;
    }

    .gallery {
		display:grid;
		grid-template-columns: repeat(auto-fill, 100px);
		grid-auto-rows: 100px;
		grid-auto-flow: dense;

	}
	.item {
		overflow: hidden;
		display: grid;
		grid-template-columns:1;
		grid-template-rows:1;
	}
	.item img {
		grid-column: 1/-1;
		grid-row: 1/-1;
		width: 100%;
		height: 100%;
		object-fit: cover;
	}
	.item__overlay {
		background: #ffc60032;
		grid-column: 1/-1;
		grid-row: 1/-1;
		position: relative;
		display: grid;
		justify-items: center;
		align-items: center;
		transition: 0.3s;
		transform: translateY(100%);
	}
	.item__overlay button {
		background: none;
		border: 2px solid white;
		color: white;
		text-transform: uppercase;
		padding: 5px;
		background: rgba(0,0,0,0.7);

	}
	.item:hover .item__overlay {
		transform: translateY(0);
	}


	.item.v2 {
		grid-row: span 2;
	}

	.item.v3 {
		grid-row: span 3;
	}

	.item.v4 {
		grid-row: span 4;
	}

	.item.h2 {
		grid-column: span 2;
	}

	.item.h3 {
		grid-column: span 3;
	}

	.item.h4 {
		grid-column: span 4;
	}



    .overlay {
      position: fixed;
      background: rgba(0, 0, 0, 0.7);
      top: 0;
      right: 0;
      bottom: 0;
      left: 0;
      display: none;
      z-index: 2;
    }

    .overlay.open {
	  display: grid;
	  align-items: center;
	  justify-items: center;

    }

    .overlay .overlay-inner {
      background: white;
      width: 700px;
      padding: 20px;
    }

    .overlay img {
      width: 100%;
    }
  </style>

<script type="text/javascript">
const gallery = document.querySelector('.gallery');
const overlay = document.querySelector('.overlay');

const overlayImage = overlay.querySelector('img');
const overlayClose = overlay.querySelector('.close');

// use 12 for limit if using 12 images
function generateHTML([h,v]) {
	return `
		<div class="item h${h} v${v}">
			<img src="../images/f${randomNumber(9)}.jpg">
			<div class="item__overlay">
				<button>View + </button>
			</div>
		</div>
	`;
}

function randomNumber(limit) {
	return Math.floor(Math.random() * limit) + 1;
}

function handleClick(e) {
	const src = e.currentTarget.querySelector('img').src;
	overlayImage.src = src;
	overlay.classList.add('open');
}

function close() {
	overlay.classList.remove('open');
}



const digits = Array.from({ length: 50 }, () => [randomNumber(4), randomNumber(4)]).concat([[1, 1], [1, 1], [1, 1], [1, 1], [1, 1], [1, 1], [1, 1], [1, 1], [1, 1], [1, 1]  ]);

const html = digits.map(generateHTML).join('');
gallery.innerHTML = html;

const items = document.querySelectorAll('.item');

items.forEach(item => item.addEventListener('click', handleClick));


</script>




<div class="overlay">
	<div class="overlay-inner">
		<button class="close">× Close</button>
		<img>
	</div>
</div>

  <section class="gallery">
  </section>
  <!-- ALL images are 500x500px   -->

