from flask import Flask
import random
app = Flask(__name__)

datos= ["Las redes sociales tienen aspectos positivos y negativos, y debemos ser conscientes de ambos cuando utilicemos estas plataformas","Elon Musk también aboga por la regulación de las redes sociales y la protección de los datos personales de los usuarios. Afirma que las redes sociales recopilan una enorme cantidad de información sobre nosotros, que luego puede utilizarse para manipular nuestros pensamientos y comportamientos","Elon Musk afirma que las redes sociales están diseñadas para mantenernos dentro de la plataforma, para que pasemos el mayor tiempo posible viendo contenidos"
,"Una forma de combatir la dependencia tecnológica es buscar actividades que aporten placer y mejoren el estado de ánimo","Según un estudio de 2019, más del 60% de las personas responden a mensajes de trabajo en sus smartphones en los 15 minutos siguientes a salir del trabajo","La mayoría de las personas que sufren adicción tecnológica experimentan un fuerte estrés cuando se encuentran fuera del área de cobertura de la red o no pueden utilizar sus dispositivos","Según un estudio realizado en 2018, más del 50% de las personas de entre 18 y 34 años se consideran dependientes de sus smartphones.","El estudio de la dependencia tecnológica es una de las áreas más relevantes de la investigación científica moderna"]


@app.route("/")
def hello_world():
    return f'<h1>Bienvenido a mi pagina wb usando flask<h1> <a href="/datos_aleatorios">Ir a ver los'


@app.route("/datos_aleatorios")
def datosaleatorios():
    return f'<h1>{random.choice(datos)}</h1>'

@app.route("/Video")
def Video():
    return f' <h1>Aqui Te Pongo dos Enlaces de videos<h1> <a href="/Video,"https://www.youtube.com/watch?v=wHkj1qLUtfk","https://www.youtube.com/watch?v=WMEk-bua9vA&t=1s">  
 

app.run(debug=True)
