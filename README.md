<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Societe Pro Z</title>
<style>
body { margin:0; font-family: Arial, sans-serif; background-color: #000; color: #fff; }
a { color: #fff; text-decoration: none; }
header, footer { background-color: #111; padding: 20px; }
nav a { margin: 0 10px; }
section { padding: 60px 20px; max-width: 1000px; margin: auto; }
h1, h2 { color: #fff; }
.contact-info div { margin-bottom: 10px; }
input, textarea { width: 100%; padding: 10px; margin-top:5px; background-color: #222; border: 1px solid #444; color: #fff; }
button { padding: 10px 20px; margin-top:10px; background-color:#333; color:#fff; border:none; cursor:pointer; }
button:hover { background-color:#555; }
.services, .portfolio { display: flex; flex-wrap: wrap; gap: 20px; }
.service-card, .portfolio-item { background-color:#111; padding:20px; flex:1; min-width:250px; border:1px solid #444; border-radius:8px; }
img { max-width: 100%; border-radius:8px; }

/* Effets pour portfolio */
.portfolio-item img { transition: transform 0.3s; }
.portfolio-item img:hover { transform: scale(1.05); }

/* Navigation hover */
nav a:hover { color: #ff9800; }

/* Formulaire bouton amélioré */
button { background-color: #ff9800; color: #000; font-weight: bold; transition: background 0.3s; }
button:hover { background-color: #e68a00; }

/* Responsive */
@media (max-width: 768px) {
    .services, .portfolio { flex-direction: column; }
}
</style>
</head>
<body>

<!-- Header généré par JavaScript -->
<div id="header-container"></div>

<script>
  const headerHTML = `
    <header>
      <h1>Societe Pro Z</h1>
      <p>Entreprise générale du batiment</p>
      <nav>
        <a href="#about">À propos</a>
        <a href="#services">Services</a>
        <a href="#portfolio">Portfolio</a>
        <a href="#contact">Contact</a>
      </nav>
    </header>
  `;
  document.getElementById('header-container').innerHTML = headerHTML;
</script>

<section id="about">
<h2>À propos</h2>
<p>Societe Pro Z est une entreprise générale du bâtiment basée à Frépillon. Nous intervenons sur tous types de travaux de construction et rénovation, avec un engagement pour la qualité et le respect des délais.</p>
</section>

<section id="services">
<h2>Services</h2>
<div class="services">
<div class="service-card"><h3>Construction</h3><p>Bâtiments résidentiels et commerciaux.</p></div>
<div class="service-card"><h3>Rénovation</h3><p>Réhabilitation et remise à neuf de vos locaux.</p></div>
<div class="service-card"><h3>Travaux divers</h3><p>Petits et grands travaux de maçonnerie et gros oeuvre.</p></div>
</div>
</section>

<section id="portfolio">
<h2>Portfolio</h2>
<div class="portfolio">
<div class="portfolio-item"><img src="https://picsum.photos/400/300?random=1" alt="Projet 1"><p>Projet 1</p></div>
<div class="portfolio-item"><img src="https://picsum.photos/400/300?random=2" alt="Projet 2"><p>Projet 2</p></div>
<div class="portfolio-item"><img src="https://picsum.photos/400/300?random=3" alt="Projet 3"><p>Projet 3</p></div>
</div>
</section>

<section id="contact">
<h2>Contact</h2>
<div class="contact-info">
<div>Téléphone: 07 52 24 43 91</div>
<div>Email: mohamedzidi1604@gmail.com</div>
<div>Adresse: 37 rue de France, Frépillon 95740</div>
</div>
<form>
<label>Nom</label>
<input type="text" placeholder="Votre nom">
<label>Email</label>
<input type="email" placeholder="Votre email">
<label>Message</label>
<textarea rows="5" placeholder="Votre message"></textarea>
<button type="submit">Envoyer</button>
</form>
</section>

<footer>
<p>© 2025 Societe Pro Z — Tous droits réservés</p>
</footer>

</body>
</html>
