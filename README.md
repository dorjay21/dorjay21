<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>AJICEF – Plateforme Intégrée</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <style>
    :root {
      --ajicef-bleu: #005a9c;
      --ajicef-or: #f5a623;
      --ajicef-vert: #4caf50;
      --bg-light: #f9f9f9;
      --text-color: #333;
      --white: #fff;
    }

    body {
      font-family: 'Segoe UI', Roboto, sans-serif;
      background-color: var(--bg-light);
      color: var(--text-color);
      margin: 0;
      padding: 0;
    }

    header {
      background-color: var(--ajicef-bleu);
      color: var(--white);
      padding: 1rem;
    }

    nav {
      display: flex;
      justify-content: space-around;
      flex-wrap: wrap;
    }

    nav a {
      color: var(--white);
      text-decoration: none;
      padding: 0.5rem;
    }

    nav a:hover {
      text-decoration: underline;
    }

    .container {
      max-width: 1200px;
      margin: auto;
      padding: 1rem;
    }

    h1, h2, h3 {
      color: var(--ajicef-bleu);
    }

    section {
      background-color: var(--white);
      border-left: 5px solid var(--ajicef-or);
      padding: 1rem;
      margin-bottom: 1.5rem;
      box-shadow: 0 0 8px rgba(0,0,0,0.05);
    }

    form {
      display: flex;
      flex-direction: column;
      gap: 0.5rem;
      max-width: 500px;
      margin: 1rem 0;
    }

    form input, form textarea, form select {
      padding: 0.6rem;
      border: 1px solid #ccc;
      border-radius: 4px;
    }

    button, .btn {
      background-color: var(--ajicef-vert);
      color: var(--white);
      padding: 0.6rem 1.2rem;
      border: none;
      border-radius: 4px;
      cursor: pointer;
      text-transform: uppercase;
    }

    button:hover {
      background-color: #388e3c;
    }

    .multi-page {
      display: flex;
      flex-direction: column;
      gap: 1rem;
      margin-top: 2rem;
    }

    .multi-page a {
      background-color: var(--ajicef-or);
      padding: 0.5rem 1rem;
      border-radius: 4px;
      color: var(--white);
      text-decoration: none;
      width: fit-content;
    }

    .multi-page a:hover {
      background-color: #d48820;
    }
  </style>
</head>
<body>
  <header>
    <h1>AJICEF</h1>
    <nav>
      <a href="#accueil">Accueil</a>
      <a href="#boutique">Boutique</a>
      <a href="#articles">Articles</a>
      <a href="#espace-membre">Espace Membre</a>
      <a href="#apropos">À propos</a>
      <a href="#galerie">Galerie</a>
      <a href="#archives">Archives</a>
      <a href="#newsletter">Newsletter</a>
      <a href="#admin">Admin</a>
    </nav>
  </header>

  <div class="container">
    <section id="accueil">
      <h2>Bienvenue à l'AJICEF</h2>
      <p>L'Association des Jeunes Intellectuels pour la Culture, l'Émergence et la Formation vous accueille. Découvrez nos concours, nos activités, et comment participer à notre engagement citoyen.</p>
    </section>

    <section id="boutique">
      <h2>Boutique AJICEF</h2>
      <p>Découvrez nos articles et produits culturels.</p>
      <form>
        <input type="text" placeholder="Nom du produit">
        <input type="number" placeholder="Quantité">
        <button type="submit">Ajouter au panier</button>
      </form>
    </section>

    <section id="articles">
      <h2>Articles récents</h2>
      <p>Explorez nos réflexions et publications sur la jeunesse et le développement.</p>
    </section>

    <section id="espace-membre">
      <h2>Espace Membre</h2>
      <form>
        <input type="email" placeholder="Email">
        <input type="password" placeholder="Mot de passe">
        <button type="submit">Connexion</button>
      </form>
      <div class="multi-page">
        <a href="#reservations">Mes Réservations</a>
        <a href="#commandes">Mes Commandes</a>
        <a href="#paiements">Infos & Paiements</a>
        <a href="#adresses">Mes Adresses</a>
        <a href="#abonnements">Mes Abonnements</a>
        <a href="#compte">Mon Compte</a>
      </div>
    </section>

    <section id="reservations">
      <h3>Réservations</h3>
      <form>
        <input type="text" placeholder="Nom de l'activité">
        <input type="date">
        <button type="submit">Réserver</button>
      </form>
    </section>

    <section id="commandes">
      <h3>Commandes</h3>
      <p>Vos commandes récentes apparaîtront ici.</p>
    </section>

    <section id="paiements">
      <h3>Paiements</h3>
      <p>Informations de paiement et factures.</p>
    </section>

    <section id="adresses">
      <h3>Adresses</h3>
      <p>Ajoutez ou modifiez vos adresses de livraison.</p>
    </section>

    <section id="abonnements">
      <h3>Abonnements</h3>
      <p>Gérez vos abonnements AJICEF.</p>
    </section>

    <section id="compte">
      <h3>Mon Compte</h3>
      <p>Modifier votre profil et mot de passe.</p>
    </section>

    <section id="apropos">
      <h2>À propos</h2>
      <p>Notre mission, nos valeurs et notre vision pour la jeunesse haïtienne.</p>
    </section>

    <section id="galerie">
      <h2>Galerie</h2>
      <p>Photos de nos événements et concours.</p>
    </section>

    <section id="archives">
      <h2>Archives</h2>
      <p>Retrouvez nos anciens projets et bulletins.</p>
    </section>

    <section id="newsletter">
      <h2>Inscription à la Newsletter</h2>
      <form>
        <input type="email" placeholder="Votre email">
        <button type="submit">S'inscrire</button>
      </form>
    </section>

    <section id="admin">
      <h2>Admin</h2>
      <form>
        <input type="text" placeholder="Nom d'utilisateur">
        <input type="password" placeholder="Mot de passe">
        <button type="submit">Connexion Admin</button>
      </form>
    </section>
  </div>

  <footer style="background-color: var(--ajicef-bleu); color: white; text-align: center; padding: 1rem;">
    © 2025 AJICEF – Tous droits réservés
  </footer>
</body>
</html>
