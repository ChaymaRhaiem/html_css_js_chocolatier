
document.addEventListener("DOMContentLoaded", () => {
  /* Catch user click event on anywhere on the page */
  document.querySelector('body').addEventListener('click', e => {
    /* Close all the dropdowns */
    document.querySelectorAll('.dropdown.open').forEach(item => {
      item.classList.remove('open');
    });
  });

  //vgbtbtrty

  /* Get all the dropdowns on the page */
  document.querySelectorAll('.dropdown').forEach(item => {
    /*
        When user clicks on a dropdown => then toggle the .open class.
        .open class is responsible for opening / closing a dropdown
*/
    item.addEventListener('click', e => {
      e.preventDefault();
      e.stopPropagation();
      /* Find the closest dropdown */
      const dropdown = e.target.closest('.dropdown');
      if (!dropdown) return;
      if (dropdown.classList.contains('open')) {
        dropdown.classList.remove('open');
      } else {
        dropdown.classList.add('open');
      }
    });
  });
});



$(document).ready(function () {
  $('.dropdown').click(function (e) {
    $(this).find('.header__submenu').toggleClass('open');
    $($(e.target).find('.down-caret').toggleClass('open-caret'));
    e.preventDefault();
    e.stopPropagation();
    $(document).click(function () {
      $('.dropdown-menu').removeClass('open');
      $('.down-caret').removeClass('open-caret');
    });
  });
});


$(".btn-2").click(function () {
  ev.preventDefault();
  $('.search__btn').removeClass('hide');
  $('.btn-2').addClass('hide');
});





function change() {

  var btn = document.getElementById("swap-btn");

  if (btn.value == "Show category") {
    btn.value = "Show filter";
    btn.innerHTML = "Show filter";
  }
  else {
    btn.value = "Show category";
    btn.innerHTML = "Show category";
  }

}


$(".dropdown-menu").on("change", "input[type='checkbox']", function () {
  $(this).closest("li").toggleClass("active", this.checked);
});




categorySelection("all")
function categorySelection(s) {
  var x, i;
  x = document.getElementsByClassName("categorydiv");
  if (s == "all") s = "";
  // Add the "show" class (display:block) to the filtered elements, and remove the "show" class from the elements that are not selected
  for (i = 0; i < x.length; i++) {
    w3RemoveClass(x[i], "show");
    if (x[i].className.indexOf(s) > -1) w3AddClass(x[i], "show");
  }
}







filterSelection("all")
function filterSelection(c) {
  var x, i;
  x = document.getElementsByClassName("filterDiv");
  if (c == "all") c = "";
  // Add the "show" class (display:block) to the filtered elements, and remove the "show" class from the elements that are not selected
  for (i = 0; i < x.length; i++) {
    w3RemoveClass(x[i], "show");
    if (x[i].className.indexOf(c) > -1) w3AddClass(x[i], "show");
  }
}

// Show filtered elements
function w3AddClass(element, name) {
  var i, arr1, arr2;
  arr1 = element.className.split(" ");
  arr2 = name.split(" ");
  for (i = 0; i < arr2.length; i++) {
    if (arr1.indexOf(arr2[i]) == -1) {
      element.className += " " + arr2[i];
    }
  }
}


// Hide elements that are not selected
function w3RemoveClass(element, name) {
  var i, arr1, arr2;
  arr1 = element.className.split(" ");
  arr2 = name.split(" ");
  for (i = 0; i < arr2.length; i++) {
    while (arr1.indexOf(arr2[i]) > -1) {
      arr1.splice(arr1.indexOf(arr2[i]), 1);
    }
  }
  element.className = arr1.join(" ");
}
/*
// Add active class to the current control button (highlight it)
var btnContainer = document.getElementById("myBtnContainer");
var btns = btnContainer.getElementsByClassName("btn");
for (var i = 0; i < btns.length; i++) {
  btns[i].addEventListener("click", function () {
    var current = document.getElementsByClassName("active");
    current[0].className = current[0].className.replace(" active", "");
    this.className += " active";
  });
}
*/

function toggle() {
  var x = document.getElementById("cart-region");
  if (x.style.display === "none") {
    x.style.display = "block";
  } else {
    x.style.display = "none";
  }
}


function toggle__diet() {
  var x = document.getElementById("useful__info");
  if (x.style.display === "none") {
    x.style.display = "block";
  } else {
    x.style.display = "none";
  }
}

function increment() {
  $('.cart__quantity-value').val( function(i, oldval) {
      return ++oldval;
  });
}


function decrement() {
  $('.cart__quantity-value').val( function(i, oldval) {
      return --oldval;
  });
}


