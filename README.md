# Aveunture
web de viajes
# Aveunture
<!-- HERO SLIDER CON FILTROS DE BÚSQUEDA DINÁMICOS -->
<div class="hero-slider-full">
  <!-- Slide 1 -->
  <div class="slide active" style="background-image: url('https://aventuremundiando.com/wp-content/uploads/2025/07/portada1.png');">
    <div class="contenido">
      <h1>Explora Colombia</h1>
      <p>Desde nevados hasta selva. Aventuras que te transforman.</p>
      <a href="https://aventuremundiando.com/destinations/montana/" class="btn-reserva" target="_blank">Reserva tu viaje</a>
    </div>
  </div>

  <!-- Slide 2 -->
  <div class="slide" style="background-image: url('https://aventuremundiando.com/wp-content/uploads/2025/07/portada-3.png');">
    <div class="contenido">
      <h1>Descubre la Amazonía</h1>
      <p>Naturaleza salvaje, cultura ancestral.</p>
      <a href="https://aventuremundiando.com/destinations/planes-colombia/" class="btn-reserva" target="_blank">Ver Amazonas</a>
    </div>
  </div>

  <!-- Slide 3 -->
  <div class="slide" style="background-image: url('https://aventuremundiando.com/wp-content/uploads/2025/07/portada-4.png');">
    <div class="contenido">
      <h1>Relájate en el Caribe</h1>
      <p>Playas cristalinas y paisajes inolvidables.</p>
      <a href="https://aventuremundiando.com/destinations/playa-aventour/" class="btn-reserva" target="_blank">Ir al Caribe</a>
    </div>
  </div>

  <!-- Slide 4 -->
  <div class="slide" style="background-image: url('https://aventuremundiando.com/wp-content/uploads/2024/10/urrao.jpeg');">
    <div class="contenido">
      <h1>Colores de vida</h1>
      <p>Biodiversidad única en cada rincón.</p>
      <a href="https://aventuremundiando.com/destinations/senderismo/" class="btn-reserva" target="_blank">Ver naturaleza</a>
    </div>
  </div>

  <!-- Slide 5 -->
  <div class="slide" style="background-image: url('https://aventuremundiando.com/wp-content/uploads/2025/07/portada-2.png');">
    <div class="contenido">
      <h1>Adrenalina pura</h1>
      <p>Viajes extremos en lugares asombrosos.</p>
      <a href="https://aventuremundiando.com/destinations/deportes-extremos/" class="btn-reserva" target="_blank">Explorar aventuras</a>
    </div>
  </div>

  <!-- Slide 6 -->
  <div class="slide" style="background-image: url('https://aventuremundiando.com/wp-content/uploads/2025/07/Calles-Coloniales-en-Colombia.png');">
    <div class="contenido">
      <h1>Encanto de los pueblos</h1>
      <p>Tradición, historia y gente cálida.</p>
      <a href="https://aventuremundiando.com/destinations/planes-colombia/" class="btn-reserva" target="_blank">Ver pueblos</a>
    </div>
  </div>
</div>


<!-- FILTRO DE BUSQUEDA INTERACTIVO -->
<div class="barra-filtros-h">
  <div class="contenedor-filtros">
    <!-- Selector por ubicación -->
    <select name="ubicacion">
      <option value="">Ubicación</option>
      <option value="bogota">Bogotá</option>
      <option value="medellin">Medellín</option>
      <option value="amazonas">Amazonas</option>
      <option value="santamarta">Santa Marta</option>
    </select>

    <!-- Selector por categoría -->
    <select name="categoria">
      <option value="">Categoría</option>
      <option value="aventura">Aventura</option>
      <option value="familiar">Familiar</option>
      <option value="extremos">Extremos</option>
      <option value="altamontaña">AltaMontaña</option>
      <option value="trepacerros">TrepaCerros</option>
    </select>

    <!-- Selector por dificultad -->
    <select name="dificultad">
      <option value="">Dificultad</option>
      <option value="facil">Fácil</option>
      <option value="media">Media</option>
      <option value="alta">Alta</option>
    </select>

    <!-- Selector por fecha -->
    <select name="fecha">
      <option value="">Fecha</option>
      <option value="2025-07">Julio 2025</option>
      <option value="2025-08">Agosto 2025</option>
      <option value="2025-09">Septiembre 2025</option>
      <option value="2025-10">Octubre 2025</option>
      <option value="2025-11">Noviembre 2025</option>
      <option value="2025-12">Diciembre 2025</option>
    </select>

    <!-- Botón para aplicar filtros -->
    <button>Aplicar</button>
  </div>
</div>

<!-- ESTILOS CSS PERSONALIZADOS -->
<style>
/* Estilos generales del slider */
.hero-slider-full {
  width: 100vw;
  height: 100vh;
  margin-left: calc(-50vw + 50%);
  overflow: hidden;
  position: relative;
}

.slide {
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0; left: 0;
  background-size: cover;
  background-position: center;
  opacity: 0;
  transition: opacity 1.5s ease-in-out;
  display: flex;
  align-items: center;
  justify-content: center;
}

.slide.active {
  opacity: 1;
  z-index: 1;
}

/* Contenido dentro del slider */
.contenido {
  background-color: rgba(0, 0, 0, 0.5);
  padding: 30px;
  border-radius: 12px;
  text-align: center;
  color: #fff;
  max-width: 90%;
  box-shadow: 0 0 15px rgba(0,0,0,0.3);
}

.contenido h1 {
  font-size: 3em;
  margin-bottom: 10px;
  color: #e3ffde;
}

.contenido p {
  font-size: 1.3em;
  margin-bottom: 20px;
}

/* Botón de llamado a la acción */
.btn-reserva {
  background-color: #fdd835;
  color: #000;
  padding: 12px 25px;
  border-radius: 8px;
  text-decoration: none;
  font-weight: bold;
  transition: background 0.3s ease;
}

.btn-reserva:hover {
  background-color: #ffca28;
  color: #222;
}

/* Filtros horizontales */
.barra-filtros-h {
  width: 100vw;
  margin-left: calc(-50vw + 50%);
  background-color: #2e2e2e;
  padding: 20px 0;
  overflow-x: auto;
}

.contenedor-filtros {
  display: flex;
  gap: 15px;
  align-items: center;
  flex-wrap: nowrap;
  overflow-x: auto;
  padding: 0 20px;
}

.contenedor-filtros select,
.contenedor-filtros button {
  background-color: #3a3a3a;
  color: white;
  border: none;
  border-radius: 8px;
  padding: 10px 15px;
  font-size: 1em;
  min-width: 160px;
  white-space: nowrap;
}

.contenedor-filtros button {
  background-color: transparent;
  border: 2px solid #ff9900;
  color: #ff9900;
  font-weight: bold;
  transition: 0.3s ease;
}

.contenedor-filtros button:hover {
  background-color: #ff9900;
  color: #000;
}

/* Responsivo */
@media screen and (max-width: 768px) {
  .hero-slider-full {
    height: 80vh;
  }

  .contenido h1 {
    font-size: 1.8em;
  }

  .contenido p {
    font-size: 1em;
  }

  .btn-reserva {
    font-size: 0.95em;
    padding: 10px 20px;
  }

  .barra-filtros-h {
    padding: 10px 0;
  }

  .contenedor-filtros {
    gap: 10px;
    padding: 0 10px;
  }

  .contenedor-filtros select,
  .contenedor-filtros button {
    font-size: 0.9em;
    min-width: 140px;
    padding: 8px 10px;
  }
}
</style>

<!-- JAVASCRIPT PARA CAMBIAR SLIDES AUTOMÁTICAMENTE -->
<script>
let currentSlide = 0;
const slides = document.querySelectorAll('.hero-slider-full .slide');

function showNextSlide() {
  slides[currentSlide].classList.remove('active');
  currentSlide = (currentSlide + 1) % slides.length;
  slides[currentSlide].classList.add('active');
}

setInterval(showNextSlide, 5000); // cambia de slide cada 5 segundos
</script>

<!-- JAVASCRIPT PARA FILTRO Y REDIRECCIÓN DINÁMICA -->
<script>
document.querySelector(".contenedor-filtros button").addEventListener("click", function () {
  const ubicacion = document.querySelector('select[name="ubicacion"]').value;
  const categoria = document.querySelector('select[name="categoria"]').value;
  const dificultad = document.querySelector('select[name="dificultad"]').value;
  const fecha = document.querySelector('select[name="fecha"]').value;

  // Define la URL base según la categoría seleccionada
  let baseUrl = "https://aventuremundiando.com";

  switch (categoria) {
    case "aventura":
    case "familiar":
      baseUrl += "/destinations/planes-colombia/";
      break;
    case "extremos":
      baseUrl += "/destinations/deportes-extremos/";
      break;
    case "altamontaña":
      baseUrl += "/destinations/montana/";
      break;
    case "trepacerros":
      baseUrl += "/destinations/senderismo/";
      break;
    default:
      baseUrl += "/destinations/";
  }

  // Construye la URL con parámetros
  const url = `${baseUrl}?ubicacion=${ubicacion}&dificultad=${dificultad}&fecha=${fecha}`;
  window.location.href = url; // Redirige a la URL filtrada
});
</script>


<!-- ¿Qué hace todo esto?
Muestra un slider de pantalla completa con contenido inspirador.

Cada slide lleva a una sección temática de tu web.

Debajo del slider, hay un filtro dinámico (ubicación, categoría, dificultad, fecha).






Al hacer clic en "Aplicar", redirige automáticamente a una URL personalizada según las opciones seleccionadas. -->
