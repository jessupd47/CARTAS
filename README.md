class TarjetaAI:
    def __init__(self):
        self.saludos = ["Querido/a", "Estimado/a", "Hola"]
        self.ocasiones = ["cumpleaños", "aniversario", "graduación", "boda", "nacimiento", "condolencias", "agradecimiento", "amistad", "Día de la Madre", "Día del Padre", "Día de San Valentín"]
        self.mensajes = ["¡Que tengas un día maravilloso!", "¡Felicidades!", "¡Te deseamos lo mejor!", "Estamos contigo en este momento difícil.", "Gracias por todo lo que haces.", "Te apreciamos mucho."]
    
    def crear_tarjeta(self, destinatario, ocasion):
        import random
        saludo = random.choice(self.saludos)
        mensaje = random.choice(self.mensajes)
        return f"{saludo} {destinatario},\n\nFeliz {ocasion}.\n{mensaje}\n\nAtentamente,\n[Tu Nombre]"

# Ejemplo de uso:
tarjeta_ai = TarjetaAI()
destinatario = "Ana"
ocasion = "cumpleaños"
tarjeta = tarjeta_ai.crear_tarjeta(destinatario, ocasion)
print(tarjeta)

