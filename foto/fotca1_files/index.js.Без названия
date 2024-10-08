
const slider = document.querySelector('.gallery');
let isDown = false;
let startX;
let scrollLeft;

slider.addEventListener('mousedown', e => {
  isDown = true;
  slider.classList.add('active');
  startX = e.pageX - slider.offsetLeft;
  scrollLeft = slider.scrollLeft;
});
slider.addEventListener('mouseleave', _ => {
  isDown = false;
  slider.classList.remove('active');
});
slider.addEventListener('mouseup', _ => {
  isDown = false;
  slider.classList.remove('active');
});
slider.addEventListener('mousemove', e => {
  if (!isDown) return;
  e.preventDefault();
  const x = e.pageX - slider.offsetLeft;
  const SCROLL_SPEED = 3;
  const walk = (x - startX) * SCROLL_SPEED;
  slider.scrollLeft = scrollLeft - walk;
});

document.querySelector('.controls-slider.left').addEventListener('click', () => slide(-1000)) 
document.querySelector('.controls-slider.right').addEventListener('click', () => slide(1000)) 
 
function slide (pxs) { 
  scrollLeft = slider.scrollLeft 
  slider.scrollLeft = scrollLeft + pxs 
}


 // navbar burger
document.addEventListener('DOMContentLoaded', () => { 
  // Get all "navbar-burger" elements 
  const $navbarBurgers = Array.prototype.slice.call(document.querySelectorAll('.navbar-burger'), 0); 
 
  // Check if there are any navbar burgers 
  if ($navbarBurgers.length > 0) { 
 
    // Add a click event on each of them 
    $navbarBurgers.forEach( el => { 
      el.addEventListener('click', () => { 
 
        // Get the target from the "data-target" attribute 
        const target = el.dataset.target; 
        const $target = document.getElementById(target); 
 
        // Toggle the "is-active" class on both the "navbar-burger" and the "navbar-menu" 
        el.classList.toggle('is-active'); 
        $target.classList.toggle('is-active'); 
 
      }); 
    }); 
  } 
 
});



var phoneMask = IMask(
  document.getElementById('phone-mask'), {
    mask: '+{998}(00)000-00-00'
  });