<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Catalogue Concessionnaire Unreal</title>
<style>
  /* Reset */
  * {
    box-sizing: border-box;
  }
  body {
    margin: 0; 
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background: linear-gradient(135deg, #0d0d0d 0%, #1a1a1a 100%);
    color: #eee;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
  }
  header {
    background: #050505;
    border-bottom: 3px solid #00ffea;
    padding: 20px 30px;
    text-align: center;
  }
  header h1 {
    margin: 0;
    font-size: 2.8rem;
    color: #00ffea;
    text-shadow: 0 0 10px #00ffe0, 0 0 20px #00ffe0;
  }
  header p {
    margin: 6px 0 0;
    font-size: 1.1rem;
    color: #55fff2;
  }
  main {
    flex-grow: 1;
    padding: 30px 50px;
    max-width: 1200px;
    margin: 0 auto;
  }
  section.category {
    margin-bottom: 50px;
  }
  section.category h2 {
    font-size: 2rem;
    border-left: 6px solid #00ffea;
    padding-left: 12px;
    margin-bottom: 25px;
    text-transform: uppercase;
    letter-spacing: 1.2px;
    color: #00d1c1;
    text-shadow: 0 0 6px #00d1c1;
  }
  .vehicles-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 25px;
  }
  article.vehicle {
    background: #111;
    border-radius: 15px;
    overflow: hidden;
    box-shadow: 0 0 12px #00ffea88;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    display: flex;
    flex-direction: column;
  }
  article.vehicle:hover {
    transform: translateY(-8px);
    box-shadow: 0 0 20px #00ffeacc;
  }
  article.vehicle img {
    width: 100%;
    height: 170px;
    object-fit: cover;
    filter: brightness(1.05);
  }
  .vehicle-content {
    padding: 15px 20px 25px 20px;
    flex-grow: 1;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }
  .vehicle-title {
    font-size: 1.3rem;
    color: #00ffe5;
    font-weight: 700;
    margin: 0 0 8px 0;
    text-shadow: 0 0 8px #00ffe5;
  }
  .vehicle-type {
    font-style: italic;
    color: #8ef8f1;
    margin-bottom: 10px;
  }
  .vehicle-desc {
    flex-grow: 1;
    font-size: 0.9rem;
    line-height: 1.3;
    color: #c0f8f5;
  }
  .vehicle-price {
    margin-top: 15px;
    font-weight: 900;
    font-size: 1.15rem;
    color: #00ffae;
    text-shadow: 0 0 10px #00ffae;
  }
  footer {
    background: #050505;
    color: #33ffcc;
    text-align: center;
    padding: 20px 15px;
    font-size: 0.9rem;
    border-top: 3px solid #00ffea;
  }
  @media (max-width: 600px) {
    main {
      padding: 20px 15px;
    }
    article.vehicle img {
      height: 140px;
    }
  }
</style>
</head>
<body>

<header>
  <h1>Concessionnaire Unreal</h1>
  <p>Catalogue officiel des véhicules Unreal – Sport, SUV & Moto</p>
</header>

<main>

  <!-- Catégorie Sport -->
  <section class="category" id="sport">
    <h2>Sport</h2>
    <div class="vehicles-grid">

      <article class="vehicle">
        <img src="https://cdn.pixabay.com/photo/2016/03/27/21/59/auto-1283104_1280.jpg" alt="Lightning ZX" />
        <div class="vehicle-content">
          <h3 class="vehicle-title">Lightning ZX</h3>
          <div class="vehicle-type">Voiture Sportive – 2 places</div>
          <p class="vehicle-desc">
            Voiture ultra rapide équipée d’un moteur électrique dernière génération. Maniabilité et accélération au top pour dominer la route.
          </p>
          <div class="vehicle-price">Prix : 120 000 $</div>
        </div>
      </article>

      <article class="vehicle">
        <img src="https://cdn.pixabay.com/photo/2021/08/10/18/54/sportscar-6533845_1280.jpg" alt="Nebula GT" />
        <div class="vehicle-content">
          <h3 class="vehicle-title">Nebula GT</h3>
          <div class="vehicle-type">Voiture Supercar – 2 places</div>
          <p class="vehicle-desc">
            Supercar avec design futuriste et performances extrêmes. Accélération fulgurante et tenue de route impeccable.
          </p>
          <div class="vehicle-price">Prix : 250 000 $</div>
        </div>
      </article>

      <article class="vehicle">
        <img src="https://cdn.pixabay.com/photo/2021/12/22/20/50/sports-car-6887607_1280.jpg" alt="Vortex RS" />
        <div class="vehicle-content">
          <h3 class="vehicle-title">Vortex RS</h3>
          <div class="vehicle-type">Voiture Sportive – 2 places</div>
          <p class="vehicle-desc">
            Véritable bijou de technologie alliant puissance et élégance. Parfait pour les amateurs de vitesse et de design.
          </p>
          <div class="vehicle-price">Prix : 140 000 $</div>
        </div>
      </article>

    </div>
  </section>

  <!-- Catégorie SUV -->
  <section class="category" id="suv">
    <h2>SUV & Tout-Terrain</h2>
    <div class="vehicles-grid">

      <article class="vehicle">
        <img src="https://cdn.pixabay.com/photo/2017/07/31/11/28/jeep-2553123_1280.jpg" alt="Terra Ranger" />
        <div class="vehicle-content">
          <h3 class="vehicle-title">Terra Ranger</h3>
          <div class="vehicle-type">SUV Tout-Terrain – 5 places</div>
          <p class="vehicle-desc">
            SUV robuste pour affronter tous les terrains. Confort et sécurité maximale pour les sorties hors-route.
          </p>
          <div class="vehicle-price">Prix : 85 000 $</div>
        </div>
      </article>

      <article class="vehicle">
        <img src="https://cdn.pixabay.com/photo/2016/11/29/03/51/crossover-1869326_1280.jpg" alt="Echo Trail" />
        <div class="vehicle-content">
          <h3 class="vehicle-title">Echo Trail</h3>
          <div class="vehicle-type">SUV Compact – 5 places</div>
          <p class="vehicle-desc">
            SUV urbain pratique, idéal pour la ville comme pour la campagne. Consommation maîtrisée et design moderne.
          </p>
          <div class="vehicle-price">Prix : 70 000 $</div>
        </div>
      </article>

      <article class="vehicle">
        <img src="https://cdn.pixabay.com/photo/2017/01/22/19/45/suv-2006262_1280.jpg" alt="Sentinel X" />
        <div class="vehicle-content">
          <h3 class="vehicle-title">Sentinel X</h3>
          <div class="vehicle-type">SUV Sportif – 5 places</div>
          <p class="vehicle-desc">
            SUV au look agressif et motorisation puissante. Parfait pour ceux qui veulent allier style et performance.
          </p>
          <div class="vehicle-price">Prix : 110 000 $</div>
        </div>
      </article>

    </div>
  </section>

  <!-- Catégorie Moto -->
  <section class="category" id="moto">
    <h2>Motos</h2>
    <div class="vehicles-grid">

      <article class="vehicle">
        <img src="https://cdn.pixabay.com/photo/2016/11/29/05/27/motorcycle-1869676_1280.jpg" alt="Phantom Racer" />
        <div class="vehicle-content">
          <h3 class="vehicle-title">Phantom Racer</h3>
          <div class="vehicle-type">Moto Sportive – 1 place</div>
          <p class="vehicle-desc">
            Moto légère et rapide avec un design agressif. Idéale pour les courses urbaines et les balades rapides.
          </p>
          <div class="vehicle-price">Prix : 25 000 $</div>
        </div>
      </article>

      <article class="vehicle">
        <img src="https://cdn.pixabay.com/photo/2016/02/19/10/00/motorbike-1209716_1280.jpg" alt="Iron Cruiser" />
        <div class="vehicle-content">
          <h3 class="vehicle-title">Iron Cruiser</h3>
          <div class="vehicle-type">Moto Custom – 1 place</div>
          <p class="vehicle-desc">
            Moto au style classique et robuste. Parfaite pour les longues routes avec confort optimal.
          </p>
          <div class="vehicle-price">Prix : 28 000 $</div>
        </div>
      </article>

      <article class="vehicle">
        <img src="https://cdn.pixabay.com/photo/2016/04/15/11/46/motorcycle-1335732_1280.jpg" alt="Blaze Fury" />
        <div class="vehicle-content">
          <h3 class="vehicle-title">Blaze Fury</h3>
          <div class="vehicle-type">Moto Sportive – 1 place</div>
          <p class="vehicle-desc">
            Moto agile et puissante, idéale pour les passionnés de vitesse et de sensations fortes.
          </p>
          <div class="vehicle-price">Prix : 30 000 $</div>
        </div>
      </article>

    </div>
  </section>

</main>

<footer>
  © 2026 Concessionnaire Unreal – Tous droits réservés
</footer>

</body>
</html>
