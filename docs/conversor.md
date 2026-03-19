# Conversor de Imágenes a LaTeX (OCR)

Esta es una herramienta experimental integrada directamente en la página para facilitar la transcripción de fotos de apuntes, matrices y demostraciones a código LaTeX y lenguaje natural. El resultado te lo entregará formateado y listo para copiar y pegar en tu editor.

!!! warning "Límites de uso diario"
    Actualmente, el motor de inteligencia artificial funciona bajo un esquema gratuito. Esto significa que tenemos una **cantidad limitada de peticiones por día** para todos los alumnos. Si en época de parciales la herramienta se satura de fotos, es posible que el servidor devuelva un mensaje de error temporal.

!!! success "El futuro del proyecto"
    Si la herramienta resulta de utilidad, recibe el apoyo esperado y vemos que la comunidad la adopta para colaborar con los apuntes, la idea es mejorar la integración e invertir en una infraestructura sin límites de peticiones. ¡Usala y contanos qué te parece!

---

<div class="ocr-container" style="border: 1px solid var(--md-default-fg-color--lightest); padding: 1.5rem; border-radius: 8px; margin-top: 1.5rem; background-color: var(--md-default-bg-color);">
  
  <input type="file" id="imageInput" accept="image/*" style="margin-bottom: 1rem; display: block; width: 100%;">
  <button id="convertBtn" class="md-button md-button--primary">Procesar Imagen</button>
  
  <p id="loadingText" style="display: none; margin-top: 1rem; color: var(--md-primary-fg-color);">
    ⏳ Analizando la imagen en la nube... (esto puede tardar unos segundos)
  </p>
  
  <pre><code id="resultOutput" style="display: block; margin-top: 1rem; white-space: pre-wrap; min-height: 80px;">// El código aparecerá acá //</code></pre>

</div>

<script>
  document.addEventListener("DOMContentLoaded", function() {
    const btn = document.getElementById("convertBtn");
    if (!btn) return; 

    btn.addEventListener("click", async function() {
      const fileInput = document.getElementById("imageInput");
      const resultBox = document.getElementById("resultOutput");
      const loading = document.getElementById("loadingText");

      if (fileInput.files.length === 0) {
        alert("¡Falta la imagen! Seleccioná un archivo primero.");
        return;
      }

      loading.style.display = "block";
      resultBox.textContent = "";

      const formData = new FormData();
      formData.append("image", fileInput.files[0]);

      try {
        const workerUrl = "https://TU-WORKER.TU-USUARIO.workers.dev";
        
        const response = await fetch(workerUrl, {
          method: "POST",
          body: formData
        });

        const textResult = await response.text();
        
        if (!response.ok) {
            throw new Error(textResult);
        }

        resultBox.textContent = textResult;

      } catch (error) {
        resultBox.textContent = "Error de conexión: " + error.message;
      } finally {
        loading.style.display = "none";
      }
    });
  });
</script>