# 9 Projeto de Mapeamento do COVID-19 

Projeto para mapear e interpretar os dados do COVID 19 no mundo consumindo uma API ReactJS e PWA.

API Utilizada: https://coronavirus-19-api.herokuapp.com/countries
Consumindo esta API apresentamos os dados em um Dashboard.

Bibliotecas e Tecnologias Utilizadas:
- ReactJS,
- PWA,
- Material UI,

Telas do App:

![Dashboard](https://i.imgur.com/hGLubZd.png "Dashboard")

# Exemplo da Biblioteca de API

```javascript
const path = 'https://coronavirus-19-api.herokuapp.com/countries'

const headers = {
  method: 'get',
  mode: 'cors',
  cache: 'default'
}

function getCountry(country) {
  return fetch(`${path}/${country}`, headers)
    .then((response) => response.json())
    .catch(function(err){ 
      console.error('Failed retrieving information', err);
    })
}

export default {
  getCountry
}
```

## PWA do Showing COVID19 Cases

Host: https://matux-covid19.netlify.app/
