<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¡Mis 15 Años! - Estrella</title>
    <link href="estilos.css" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Montserrat:wght@300;400;600&display=swap" rel="stylesheet">
    
</head>
<body>
    <div class="fade-mask-top"></div>
    <div class="fade-mask-bottom"></div>
    <header>
        <p style="color: #e6bf72;">Le invitamos a celebrar los</p>
        <h1 style="color: #e6bf72;">15 Años</h1>
        <p style="color: #e6bf72;">de</p>
        <span class="letra-carta">Estrella Mishel Morales Flores</span>
    </header>

    <div class="container">
        
        <h3>¡Mi Gran Noche!</h3>
        <p style="font-size: 1.1rem; line-height: 1.6;">Hay momentos en la vida que son inolvidables, y compartirlos con quienes más queremos los hace aún más especiales. ¡Acompáñame en esta noche mágica!</p>

        <div class="countdown-container" id="countdown">
            <div class="time-box"><span id="days">00</span><small>Días</small></div>
            <div class="time-box"><span id="hours">00</span><small>Horas</small></div>
            <div class="time-box"><span id="minutes">00</span><small>Min</small></div>
            <div class="time-box"><span id="seconds">00</span><small>Seg</small></div>
        </div>

        <div class="calendar-card">
            <h3>Reserva la Fecha</h3>

            <div class="calendar">
                <div class="calendar-header">
                    Junio 2026
                </div>

                <div class="calendar-days">
                    <span>Do</span>
                    <span>Lu</span>
                    <span>Ma</span>
                    <span>Mi</span>
                    <span>Ju</span>
                    <span>Vi</span>
                    <span>Sá</span>
                </div>

                <div class="calendar-grid">
                    <span></span>
                    <span>1</span>
                    <span>2</span>
                    <span>3</span>
                    <span>4</span>
                    <span>5</span>
                    <span>6</span>

                    <span>7</span>
                    <span>8</span>
                    <span>9</span>
                    <span>10</span>
                    <span>11</span>
                    <span>12</span>
                    <span>13</span>

                    <span>14</span>
                    <span>15</span>
                    <span>16</span>
                    <span>17</span>
                    <span>18</span>
                    <span>19</span>
                    <span>20</span>

                    <span>21</span>
                    <span>22</span>
                    <span>23</span>
                    <span>24</span>
                    <span>25</span>
                    <span>26</span>

                    <span class="selected-day">27</span>

                    <span>28</span>
                    <span>29</span>
                    <span>30</span>
                </div>
            </div>
        </div>

        <div class="card">
            <h2>La Celebración</h2>
            <p><strong>Fecha:</strong> Sábado, 27 de junio de 2026</p>
            <p><strong>Recepción:</strong> 16:00 hrs.</p>
            <p><strong>Lugar:</strong> Salón Municipal, Cabecera Municipal</p>
            <a href="https://maps.google.com" target="_blank" class="btn">Cómo llegar con Google Maps</a>
            <!-- <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2435.698083737473!2d-89.6514589193645!3d16.640615719075434!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x8f5fdd002a3dc351%3A0x7c58bf0946a41da7!2sSALON%20MUNICIPAL%20EL%20CHAL%2C%20PETEN!5e0!3m2!1ses!2sgt!4v1780543555290!5m2!1ses!2sgt" width="400" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe> -->
        </div>

        <div class="card">
            <h2>Código de Vestimenta</h2>
            <p style="font-size: 1.2rem; letter-spacing: 1px; color: #b8882a;"><strong>Formal / Gala</strong></p>
            <p><i>Tu mejor gala para compartir una noche inolvidable.</i></p>
        </div>

        <div class="card">
            <h2>Mesa de Regalos</h2>
            <p>El mejor regalo es contar con tu presencia. Si deseas tener un detalle conmigo, dispondremos de un cofre para sobres en la recepción o puedes realizar una transferencia bancaria:</p>
            <p style="margin-top: 20px;"><strong>Banco:</strong> Banco Central</p>
            <p><strong>Cuenta / CBU:</strong> 0000000000000000000000</p>
            <p><strong>A nombre de:</strong> Camila Pérez</p>
        </div>

    </div>

    <footer>
        <p class="letra-carta" style="font-size: 3rem; margin: 0 0 10px 0; color: #b8882a;">¡Te espero!</p>
        <p style="margin: 0; font-size: 0.85rem; opacity: 0.7;">2026 • Todos los derechos reservados</p>
    </footer>

    <script>
        // Fecha del evento: Año, Mes (Jan, Feb, Mar, Apr, May, Jun, Jul, Aug, Sep, Oct, Nov, Dec), Día, Hora
        const countDownDate = new Date("Jun 27, 2026 16:00:00").getTime();

        const x = setInterval(function() {
            const now = new Date().getTime();
            const distance = countDownDate - now;

            const days = Math.floor(distance / (1000 * 60 * 60 * 24));
            const hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
            const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
            const seconds = Math.floor((distance % (1000 * 60)) / 1000);

            document.getElementById("days").innerHTML = days < 10 ? "0" + days : days;
            document.getElementById("hours").innerHTML = hours < 10 ? "0" + hours : hours;
            document.getElementById("minutes").innerHTML = minutes < 10 ? "0" + minutes : minutes;
            document.getElementById("seconds").innerHTML = seconds < 10 ? "0" + seconds : seconds;

            if (distance < 0) {
                clearInterval(x);
                document.getElementById("countdown").innerHTML = "<h2 style='color:#dfba6b;'>¡Llegó el gran momento!</h2>";
            }
        }, 1000);
    </script>
</body>
</html>
