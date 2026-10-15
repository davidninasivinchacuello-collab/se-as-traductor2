<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover" />
  <meta name="theme-color" content="#0b3a5b" />
  <title>Puente PE — Comunicación visual</title>
  <style>
    :root {
      --bg: #f4f7fb; --card: #fff; --ink: #102033; --muted: #4d6073;
      --primary: #0b6e4f; --accent: #0b3a5b; --danger: #b42318; --line: #d5deea;
    }
    * { box-sizing: border-box; }
    body { margin: 0; font-family: "Segoe UI", system-ui, sans-serif; background: var(--bg); color: var(--ink); }
    header { background: var(--accent); color: #fff; padding: 16px; }
    header h1 { margin: 0; font-size: 1.45rem; }
    header p { margin: 6px 0 0; color: #d6e4f2; }
    main { padding: 12px; max-width: 820px; margin: 0 auto 40px; }
    .tabs { display: grid; grid-template-columns: repeat(3, 1fr); gap: 8px; margin-bottom: 12px; }
    button, textarea { font: inherit; }
    .tab, .phrase, .action, .emergency {
      border-radius: 14px; padding: 12px 8px; cursor: pointer; font-weight: 700;
    }
    .tab { background: #fff; color: var(--accent); border: 2px solid var(--line); }
    .tab.active { background: var(--accent); color: #fff; }
    .panel { display: none; }
    .panel.active { display: block; }
    .screen {
      background: #07131f; color: #f4fff8; min-height: 140px; border-radius: 18px;
      padding: 18px; font-size: 1.7rem; line-height: 1.35; font-weight: 700;
    }
    .hint { color: var(--muted); margin: 8px 2px 12px; }
    textarea {
      width: 100%; min-height: 110px; border-radius: 14px; border: 2px solid var(--line);
      padding: 14px; font-size: 1.15rem;
    }
    .row { display: flex; gap: 8px; flex-wrap: wrap; margin-top: 10px; }
    .action { background: var(--primary); color: #fff; border: none; flex: 1; min-width: 140px; }
    .action.secondary { background: #fff; color: var(--accent); border: 2px solid var(--accent); }
    .action.stop { background: var(--danger); }
    .grid { display: grid; grid-template-columns: 1fr 1fr; gap: 8px; }
    .phrase { background: #fff; border: 2px solid var(--line); text-align: left; min-height: 68px; }
    .emergency {
      background: #fff4f2; color: var(--danger); border: 2px solid #f3c1bb;
      text-align: left; width: 100%; margin-bottom: 8px;
    }
    .card, .aviso { border-radius: 16px; padding: 14px; margin-top: 12px; }
    .card { background: #fff; }
    .aviso { background: #fff7e8; border: 2px solid #e6c27a; color: #5c3b00; }
    .cam-wrap { background: #000; border-radius: 18px; overflow: hidden; margin-top: 10px; }
    video { width: 100%; max-height: 380px; object-fit: cover; transform: scaleX(-1); background: #000; }
    footer { color: var(--muted); font-size: .85rem; }
    @media (max-width: 640px) {
      .tabs { grid-template-columns: 1fr 1fr; }
      .screen { font-size: 1.4rem; }
    }
  </style>
</head>
<body>
  <header>
    <h1>Puente PE</h1>
    <p>Escribe, muestra en letras grandes, escucha y señala el significado. La cámara no traduce la LSP.</p>
  </header>
  <main>
    <div class="tabs">
      <button class="tab active" data-tab="escribir">Yo escribo</button>
      <button class="tab" data-tab="escuchar">Me hablan</button>
      <button class="tab" data-tab="frases">Frases</button>
      <button class="tab" data-tab="camara">Cámara</button>
      <button class="tab" data-tab="emergencia">Emergencia</button>
    </div>

    <div id="screen" class="screen" aria-live="polite">Hola. Escribe un mensaje y pulsa Hablar.</div>
    <p class="hint" id="status">Listo.</p>

    <section class="panel active" id="escribir">
      <textarea id="mensaje" placeholder="Escribe aquí lo que quieres decir..."></textarea>
      <div class="row">
        <button class="action" id="hablar">Hablar</button>
        <button class="action secondary" id="mostrar">Solo mostrar</button>
        <button class="action secondary" id="borrar">Borrar</button>
      </div>
    </section>

    <section class="panel" id="escuchar">
      <div class="card">
        <p>Pide que hablen cerca del micrófono. El texto aparecerá en la pantalla grande.</p>
        <div class="row">
          <button class="action" id="oir">Escuchar</button>
          <button class="action stop" id="parar">Detener</button>
        </div>
      </div>
    </section>

    <section class="panel" id="frases"><div class="grid" id="frases"></div></section>

    <section class="panel" id="camara">
      <div class="aviso">
        <strong>Esto no reconoce Lengua de Señas Peruana.</strong>
        La LSP es una lengua completa. Aquí la cámara solo ve gestos básicos (sí, no, palma, puño, dos, arriba, te quiero). Esos gestos no son señas peruanas. Si haces una seña de la LSP, elige tú el significado en los botones de abajo.
      </div>
      <div class="cam-wrap"><video id="cam" playsinline autoplay muted></video></div>
      <div class="row">
        <button class="action" id="abrirCam">Abrir cámara</button>
        <button class="action stop" id="cerrarCam">Cerrar cámara</button>
        <button class="action secondary" id="repetirGesto">Decir otra vez</button>
      </div>
      <h2>Yo elijo el significado</h2>
      <p class="hint">Pulsa lo que quieres decir. La app lo muestra y lo habla. No adivina la seña.</p>
      <div class="grid" id="significados"></div>
    </section>

    <section class="panel" id="emergencia">
      <button class="emergency" data-text="EMERGENCIA. Necesito ayuda ahora. Soy una persona sorda. Por favor escriba.">Necesito ayuda ahora</button>
      <button class="emergency" data-text="Emergencia médica. Llame al SAMU 106. No puedo oír. Por favor escriba.">Emergencia médica — SAMU 106</button>
      <button class="emergency" data-text="Necesito a la Policía. Marque 105. Soy una persona sorda. Por favor escriba.">Policía — 105</button>
      <button class="emergency" data-text="Hay un incendio o rescate. Marque a los Bomberos 116. Soy una persona sorda.">Bomberos — 116</button>
      <div class="card">
        <strong>Perú: Policía 105 · SAMU 106 · Bomberos 116</strong>
        <p>Esta app no llama sola. Muestre la pantalla o pida que marquen.</p>
      </div>
    </section>

    <footer>
      <p>Muchas personas sordas se comunican con lengua de señas peruana, escritura o voz. Esta herramienta no reemplaza a un intérprete en salud, trámites o juicios.</p>
    </footer>
  </main>
  <script>
    const FRASES = [
      "Hola, soy una persona sorda.",
      "Por favor escriba, no puedo oír.",
      "Gracias.", "Sí.", "No.",
      "No entiendo. Repita por escrito.",
      "¿Cuánto cuesta?", "¿Dónde está el baño?",
      "Necesito un intérprete de lengua de señas.",
      "Me duele aquí.", "La cuenta, por favor."
    ];
    const GESTOS = {
      Thumb_Up: "Sí",
      Thumb_Down: "No",
      Open_Palm: "Espera",
      Closed_Fist: "Atención",
      Victory: "Dos",
      Pointing_Up: "Arriba",
      ILoveYou: "Te quiero"
    };

    const screen = document.getElementById("screen");
    const status = document.getElementById("status");
    const mensaje = document.getElementById("mensaje");
    const video = document.getElementById("cam");
    let recognition = null, escuchando = false;
    let recognizer = null, camaraActiva = false, loopId = 0, ultimoTs = -1;
    let ultimoGesto = "", ultimoTiempo = 0, ultimoTexto = "";

    function mostrar(texto) {
      screen.textContent = (texto || "").trim() || "…";
    }
    function decir(texto) {
      const limpio = (texto || "").trim();
      if (!limpio || !("speechSynthesis" in window)) return;
      window.speechSynthesis.cancel();
      const u = new SpeechSynthesisUtterance(limpio);
      u.lang = "es-PE";
      u.rate = 0.95;
      window.speechSynthesis.speak(u);
    }
    function hablar(texto) {
      const limpio = (texto || "").trim();
      if (!limpio) { status.textContent = "Escribe algo antes de hablar."; return; }
      mostrar(limpio);
      ultimoTexto = limpio;
      if (!("speechSynthesis" in window)) {
        status.textContent = "Este navegador no habla. La otra persona puede leer la pantalla.";
        return;
      }
      status.textContent = "Hablando…";
      decir(limpio);
    }

    document.getElementById("hablar").onclick = () => hablar(mensaje.value);
    document.getElementById("mostrar").onclick = () => {
      mostrar(mensaje.value);
      ultimoTexto = mensaje.value.trim();
      status.textContent = "Mostrado.";
    };
    document.getElementById("borrar").onclick = () => {
      mensaje.value = "";
      mostrar("Hola. Escribe un mensaje y pulsa Hablar.");
      window.speechSynthesis.cancel();
      status.textContent = "Borrado.";
    };

    function ponerBotones(id, lista) {
      const box = document.getElementById(id);
      lista.forEach((texto) => {
        const b = document.createElement("button");
        b.className = "phrase";
        b.textContent = texto;
        b.onclick = () => { mensaje.value = texto; hablar(texto); };
        box.appendChild(b);
      });
    }
    ponerBotones("frases", FRASES);
    ponerBotones("significados", FRASES);

    document.querySelectorAll(".emergency").forEach((b) => {
      b.onclick = () => hablar(b.dataset.text);
    });
    document.querySelectorAll(".tab").forEach((tab) => {
      tab.onclick = () => {
        document.querySelectorAll(".tab").forEach((t) => t.classList.remove("active"));
        document.querySelectorAll(".panel").forEach((p) => p.classList.remove("active"));
        tab.classList.add("active");
        document.getElementById(tab.dataset.tab).classList.add("active");
      };
    });

    function crearReconocimiento() {
      const SR = window.SpeechRecognition || window.webkitSpeechRecognition;
      if (!SR) return null;
      const r = new SR();
      r.lang = "es-PE";
      r.continuous = true;
      r.interimResults = true;
      r.onresult = (e) => {
        let t = "";
        for (let i = 0; i < e.results.length; i++) t += e.results[i][0].transcript + " ";
        mostrar(t.trim());
        status.textContent = "Escuchando…";
      };
      r.onerror = () => { escuchando = false; status.textContent = "No se pudo usar el micrófono."; };
      r.onend = () => { if (escuchando) { try { r.start(); } catch (e) { escuchando = false; } } };
      return r;
    }
    document.getElementById("oir").onclick = () => {
      if (!recognition) recognition = crearReconocimiento();
      if (!recognition) { status.textContent = "Use Chrome para transcribir la voz."; return; }
      escuchando = true;
      mostrar("Escuchando…");
      try { recognition.start(); } catch (e) {}
    };
    document.getElementById("parar").onclick = () => {
      escuchando = false;
      if (recognition) recognition.stop();
      status.textContent = "Escucha detenida.";
    };

    function publicarGesto(nombre, score) {
      const texto = GESTOS[nombre];
      if (!texto || score < 0.7) return;
      const ahora = Date.now();
      if (texto === ultimoGesto && ahora - ultimoTiempo < 2500) return;
      ultimoGesto = texto;
      ultimoTiempo = ahora;
      ultimoTexto = texto;
      mostrar(texto);
      status.textContent = "Gesto básico, no es LSP: " + texto + " (" + Math.round(score * 100) + "%).";
      decir(texto);
    }

    async function cargarModelo() {
      if (recognizer) return recognizer;
      status.textContent = "Cargando detector de gestos… hace falta internet la primera vez.";
      const vision = await import("https://cdn.jsdelivr.net/npm/@mediapipe/tasks-vision@0.10.14");
      const fileset = await vision.FilesetResolver.forVisionTasks(
        "https://cdn.jsdelivr.net/npm/@mediapipe/tasks-vision@0.10.14/wasm"
      );
      const opciones = (delegate) => ({
        baseOptions: {
          modelAssetPath: "https://storage.googleapis.com/mediapipe-models/gesture_recognizer/gesture_recognizer/float16/1/gesture_recognizer.task",
          delegate
        },
        runningMode: "VIDEO",
        numHands: 1
      });
      try { recognizer = await vision.GestureRecognizer.createFromOptions(fileset, opciones("GPU")); }
      catch (e) { recognizer = await vision.GestureRecognizer.createFromOptions(fileset, opciones("CPU")); }
      return recognizer;
    }

    function bucle() {
      if (!camaraActiva) return;
      if (recognizer && video.readyState >= 2) {
        let ts = performance.now();
        if (ts <= ultimoTs) ts = ultimoTs + 1;
        ultimoTs = ts;
        try {
          const r = recognizer.recognizeForVideo(video, ts);
          const g = r.gestures && r.gestures[0] && r.gestures[0][0];
          if (g && g.categoryName !== "None") publicarGesto(g.categoryName, g.score);
        } catch (e) { status.textContent = "No se pudo leer el gesto."; }
      }
      loopId = requestAnimationFrame(bucle);
    }

    document.getElementById("abrirCam").onclick = async () => {
      if (!window.isSecureContext) {
        status.textContent = "La cámara pide HTTPS o localhost. No se abre desde un archivo suelto.";
        return;
      }
      try {
        const stream = await navigator.mediaDevices.getUserMedia({ video: { facingMode: "user" }, audio: false });
        video.srcObject = stream;
        await video.play();
        await cargarModelo();
        camaraActiva = true;
        status.textContent = "Cámara lista. Solo gestos básicos, no lengua de señas peruana.";
        bucle();
      } catch (e) {
        status.textContent = "No se pudo abrir la cámara o el modelo. Permita la cámara y revise internet.";
      }
    };
    document.getElementById("cerrarCam").onclick = () => {
      camaraActiva = false;
      cancelAnimationFrame(loopId);
      const stream = video.srcObject;
      if (stream) stream.getTracks().forEach((t) => t.stop());
      video.srcObject = null;
      status.textContent = "Cámara cerrada.";
    };
    document.getElementById("repetirGesto").onclick = () => hablar(ultimoTexto);
  </script>
</body>
</html>
