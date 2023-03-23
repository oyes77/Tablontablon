---
{"dg-publish":true,"permalink":"/daily-notes/wed-22-march-2023/","title":"DLNT","created":"2023-03-22T12:45:03.478-05:00","updated":"2023-03-23T01:34:27.300-05:00"}
---


# DLNT

```javascript
moment().format("[Today is] dddd, MMMM Do YYYY");
```

chat_id = 822595633621893150

cooldown_seconds = 15

last_triggered = 0

greetings = ["hola", "oli", "hello", "qué tal", "buenos días", "buenas tardes"]

ezm = ["Ezma", "co-owner", "dueño", "<@373569223194312714>"]

oka= ["Oka", "admon", "dueña", "<@653736251794522131>"]

@client.event

async def on_message(message):

    global last_triggered

    if message.author.bot:

        return # Ignore messages sent by bots

    if message.channel.id == chat_id and any(re.search(r"\b{}\b".format(greeting), message.content.lower()) for greeting in greetings):
        current_time = time.time()
        if current_time - last_triggered >= cooldown_seconds:
            last_triggered = current_time
            responses = ["¿Qué tal?", "¡Hola tú!", f"¡Hola {message.author.name}!", f"¡Bienvenid@ a Drawing Attack {message.author.name}!", "¡Hola!", f"¿Qué tal va tu día, {message.author.name}?", "¡Hey!", "¡Oli oli oli!", f"¡Hola {message.author.name}!", "¡Qué tal!", f"¿Cómo estás, {message.author.name}?"]
            response = random.choice(responses)
            await message.channel.send(response)

    elif message.channel.id == chat_id and any(re.search(r"\b{}\b".format(greeting), message.content.lower()) for greeting in ezm):
        current_time = time.time()
        if current_time - last_triggered >= cooldown_seconds:
            last_triggered = current_time
            responses = ["es mi papá... creo!", f"Lo necesitas?\nVEEEEN!!!! <@373569223194312714> {message.author.name} TE NECESITAAA!!!!", "Es uno de los dueños de este lugar OwO", "Está más azul de lo normal... me pregunto si estará bien T^T", "Novio de la coneja facherita", "Tal vez esté ocupado, si lo necesitas escríbele al DM", "El papu más papu de todos los papus", "El me dijo que te dijera esto...\n\n*Ponte a dibujar, desgraciado, que ese sketch no se acaba solo*", "El me dijo que te dijera esto...\n\n*Estirate, o te va a dar calambre de tula*", "El me dijo que te dijera esto...\n\n*Con paciencia y saliva...*", "El me dijo que te dijera esto...\n\n*Quien le diga algo feo a Bartolo sufrirá la ira del martillo.*"]
            response = random.choice(responses)
            await message.channel.send(response)

    elif message.channel.id == chat_id and any(re.search(r"\b{}\b".format(greeting), message.content.lower()) for greeting in oka):
        current_time = time.time()
        if current_time - last_triggered >= cooldown_seconds:
            last_triggered = current_time
            responses = ["DONDE!!!!!\n*se esconde detrás de NIXX*", "No la veo hace tiempo por aquí , la extraño T^T", "Debe estar borracha en algún rincón, si la necesitas escríbele al DM", "Novia de ChrisGOD",

- - -

Mix all the 3 variations into one event chat_id = 822595633621893150 cooldown_seconds = 15 last_triggered = 0 greetings = ["hola", "oli", "hello", "qué tal", "buenos días", "buenas tardes"] ezm = ["Ezma", "co-owner", "dueño", "<@373569223194312714>"] oka= ["Oka", "admon", "dueña", "<@653736251794522131>"] @client.event async def on_message(message): global last_triggered if message.author.bot: return # Ignore messages sent by bots if message.channel.id == chat_id and any(re.search(r"\b{}\b".format(greeting), message.content.lower()) for greeting in greetings): current_time = time.time() if current_time - last_triggered >= cooldown_seconds: last_triggered = current_time responses = ["¿Qué tal?", "¡Hola tú!", f"¡Hola {message.author.name}!", f"¡Bienvenid@ a Drawing Attack {message.author.name}!", "¡Hola!", f"¿Qué tal va tu día, {message.author.name}?", "¡Hey!", "¡Oli oli oli!", f"¡Hola {message.author.name}!", "¡Qué tal!", f"¿Cómo estás, {message.author.name}?"] response = random.choice(responses) await message.channel.send(response) await client.process_commands(message) if message.channel.id == chat_id and any(re.search(r"\b{}\b".format(greeting), message.content.lower()) for greeting in ezm): current_time = time.time() if current_time - last_triggered >= cooldown_seconds: last_triggered = current_time responses = ["es mi papá... creo!", f"Lo necesitas?\nVEEEEN!!!! <@373569223194312714> {message.author.name} TE NECESITAAA!!!!", "Es uno de los dueños de este lugar OwO", "Está más azul de lo normal... me pregunto si estará bien T^T", "Novio de la coneja facherita", "Tal vez esté ocupado, si lo necesitas escríbele al DM", "El papu más papu de todos los papus", "El me dijo que te dijera esto...\n\n*Ponte a dibujar, desgraciado, que ese sketch no se acaba solo*", "El me dijo que te dijera esto...\n\n*Estirate, o te va a dar calambre de tula*", "El me dijo que te dijera esto...\n\n*Con paciencia y saliva...*", "El me dijo que te dijera esto...\n\n*Quien le diga algo feo a Bartolo sufrirá la ira del martillo.*"] response = random.choice(responses) await message.channel.send(response) await client.process_commands(message) if message.channel.id == chat_id and any(re.search(r"\b{}\b".format(greeting), message.content.lower()) for greeting in oka): current_time = time.time() if current_time - last_triggered >= cooldown_seconds: last_triggered = current_time responses = ["DONDE!!!!!\n*se esconde detrás de NIXX*", "No la veo hace tiempo por aquí , la extraño T^T", "Debe estar borracha en algún rincón, si la necesitas escríbele al DM", "Novia de ChrisGOD", "Oka tiene el pelo blanco como la nieve!\nVen a mí, abuelita!", "Es una de los dueños de este lugar OwO", "*Sabe a Oka, pero sabe más a Okasette*"] response = random.choice(responses) await message.channel.send(response) await client.process_commands(message)

- - - 

<< [[Daily notes/Tue-21-March-2023\|Tue-21-March-2023]] | [[Daily notes/Thu-23-March-2023\|Thu-23-March-2023]] >>
