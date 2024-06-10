# Checksync

Checksync es una plataforma para controlar scrapers y mantenerlos funcionando. Es extensible, lo que permite agregar nuevos scrapers de una forma fácil y rápida. Este proyecto está dividido en tres partes: el Cliente, el Servidor y el Scraper.

## Estructura del Proyecto

1. **Cliente**: Interfaz que permite a los usuarios interactuar con los scrapers. Este componente se comunica con el Servidor para enviar y recibir datos.
2. **Servidor**: Gestiona y coordina los scrapers, asegurando que estén trabajando correctamente. Proporciona una API para que el Cliente pueda comunicarse y controlar los scrapers.
3. **Scraper**: Componentes reutilizables que se encargan de extraer información de diversas fuentes. Estos pueden ser utilizados tanto por el Cliente como por el Servidor, y es sencillo agregar nuevos scrapers a la plataforma.

## Repositorios

El proyecto Checksync se divide en tres repositorios principales:

- [Checksync Cliente](https://github.com/FrancoReyesDev/checksync-client)
- [Checksync Servidor](https://github.com/FrancoReyesDev/checksync-server)
- [Checksync Scraper](https://github.com/FrancoReyesDev/checksync-scraper)

## Instalación y Uso

### Requisitos Previos

- Node.js
- npm

### Instrucciones de Instalación

#### Cliente

1. **Clonar el repositorio del Cliente**

```
npm run build-scraper
npm install
npm run build
```
Y luego podes instalarlo global o simplemente hacer:
```
npm run start
```

#### Servidor
1. **Clonar el repositorio del Cliente**
```
npm run build-scraper
npm install
npm run build
```
En el caso del servidor podes crear un servicio para correrlo o de la forma que prefieras con:
```
npm run start
```

#### Scraper
En el caso del scraper no se debe hacer ninguna instalacion, pero para casos de testing o modificacion de algun scraper simplemente hacer:
1. **Clonar el repositorio del Cliente**
```
npm install
npm run build // buildeara un modulo instalable, dependencia del cliente y del servidor
npm run start // Correra src/test.ts


