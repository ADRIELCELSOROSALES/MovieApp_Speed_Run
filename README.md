# MovieApp

MovieApp es una aplicación Android desarrollada en Kotlin que utiliza el patrón de diseño MVVM (Model-View-ViewModel) para presentar información de películas obtenida de la API de TMDB (The Movie Database). La aplicación hace uso de Retrofit para manejar las solicitudes de red y LiveData para actualizar la UI con los datos más recientes.

## Características

- Consumo de la API de TMDB para obtener información de películas en cartelera y populares.
- Arquitectura MVVM para separar la lógica de negocio de la interfaz de usuario.
- Uso de Retrofit para las solicitudes a la API.
- Actualización de la UI en tiempo real con LiveData.

## Tecnologías Utilizadas

- Kotlin
- Retrofit
- MVVM
- LiveData
- Glide para la carga de imágenes.

![image](https://github.com/ADRIELCELSOROSALES/MovieApp_Speed_Run/assets/110257731/7bbc8a59-040d-4a9e-963e-9d9a353db234)

## Configuración

Para ejecutar este proyecto, necesitarás:

1. Clonar el repositorio:
``` git clone https://github.com/adrielcelsorosales/movieapp_speed_run.git```

2. Abrir el proyecto en Android Studio.

  
3. Obtener una API Key de TMDB y reemplazar el valor de `API_KEY` en [Constantes.kt](https://github.com/adrielcelsorosales/movieapp_speed_run/tree/main/app/src/main/java/com/example/movieapp/core/Constantes.kt).
  ``` kotlin
  object Constantes {
      const val API_KEY = "TU_API_KEY_AQUÍ"
      // Resto de constantes...
  }
  ```

4. Ejecutar la aplicación.
   
### Estructura del Proyecto
__Model:__ Define los datos que la aplicación manejará. Ejemplo: PeliculaModel.kt.

__View:__ Contiene los componentes de la UI como Activities y Adapters. Ejemplo: MainActivity.kt.

__ViewModel:__ Actúa como intermediario entre el Model y la View. Ejemplo: PeliculasViewModel.kt.

__Network:__ Gestiona las solicitudes de red utilizando Retrofit. Ejemplo: RetrofitClient.kt.


