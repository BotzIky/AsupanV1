# AsupanV1
📂 Database Asupan by [Gakkari](t.me/Gakkari)

## ```Fetch to:```
```
https://raw.githubusercontent.com/BotzIky/AsupanV1/main/database.json
```
## ```Module```
node-fetch or axios

## ```Example on the WhatsApp bot```
```
case 'asupanv1': {
    try {
        let response = await fetch('https://raw.githubusercontent.com/BotzIky/AsupanV1/main/database.json')
        let data = await response.json()
        let randomIndex = Math.floor(Math.random() * data.length)
        let randomLink = data[randomIndex]
        await client.sendMessage(from, { video: { url: randomLink } }, { quoted: m })
    } catch (error) {
        m.reply('An error occurred while fetching intake data.')
        console.error(error)
    }
}
break;
```
