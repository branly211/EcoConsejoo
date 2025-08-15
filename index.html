from flask import Flask, render_template, request, redirect, url_for, flash

app = Flask(__name__)
app.secret_key = "cambiame_por_una_clave_segura"

# Lista simple en memoria con consejos (puedes pasar a DB si quieres)
consejos = [
    {"titulo": "Ahorra agua", "texto": "Cierra el grifo mientras te cepillas los dientes y repara fugas."},
    {"titulo": "Usa transporte sostenible", "texto": "Camina, usa bicicleta o transporte público cuando sea posible."},
    {"titulo": "Reduce, reutiliza, recicla", "texto": "Evita plásticos de un solo uso y recicla en tu comunidad."},
    {"titulo": "Ahorra energía", "texto": "Apaga las luces y desconecta aparatos que no uses."}
]

@app.route("/")
def index():
    # muestra lista de consejos
    return render_template("index.html", consejos=consejos)

@app.route("/enviar", methods=["GET", "POST"])
def enviar():
    if request.method == "POST":
        titulo = request.form.get("titulo", "").strip()
        texto = request.form.get("texto", "").strip()
        if not titulo or not texto:
            flash("Por favor completa todos los campos.", "error")
            return redirect(url_for("enviar"))
        # añadir consejo (aquí en memoria; en producción guardar en DB)
        consejos.append({"titulo": titulo, "texto": texto})
        flash("¡Gracias! Tu consejo ha sido enviado.", "success")
        return redirect(url_for("index"))
    return render_template("enviar.html")

if __name__ == "__main__":
    app.run(debug=True)
