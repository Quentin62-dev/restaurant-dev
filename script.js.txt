// Message quand on clique sur le bouton
document.querySelector("button").addEventListener("click", function() {
alert("Commande bientôt disponible !");
});

// Scroll fluide vers les sections
document.querySelectorAll("nav a").forEach(link => {
link.addEventListener("click", function(e) {
e.preventDefault();

```
const target = document.querySelector(this.getAttribute("href"));

if (target) {
  target.scrollIntoView({
    behavior: "smooth"
  });
}
```

});
});
