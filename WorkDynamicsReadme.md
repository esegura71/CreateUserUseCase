# Dinamica de trabajo

<div display="flex" flex-direction-row>
<img src="laravel-2.svg" alt="Laravel Logo" width="100" height="50">
<img src="php.svg" alt="php" width="100" height="50">
<img src="docker.svg" alt="docker" width="100" height="50">
<img src="github-mark.svg" alt="github" width="50" height="50">
</div>

## Descripción del Proyecto

El objetivo principal de esta dinámica es que cada participante suba un nuevo proyecto utilizando la versión más
reciente de Laravel y PHP 8.2. La tarea inicial consistirá en implementar un único caso de uso: Crear Usuario (
CreateUser). Cada participante utilizará sus conocimientos actuales de métodos y arquitecturas.

A partir de este punto, nos embarcaremos en un viaje de refactorización, mejorando el código en cada sesión hasta
alcanzar una implementación robusta y eficiente, empleando las arquitecturas clave mencionadas.

## Duración del Proyecto

La dinámica está programada para un mes de trabajo, con 12 sesiones planificadas. Cada sesión tendrá una duración de 1 a
1.30 minutos, proporcionando el tiempo adecuado para revisar, discutir y mejorar el código.

## Nivel de Complejidad

Este proyecto está diseñado con un nivel de complejidad avanzado para desafiar y enriquecer tus habilidades de
desarrollo. Aprovecharemos las últimas versiones de Laravel y PHP para garantizar que estés al tanto de las últimas
prácticas y tendencias en el mundo del desarrollo web.

#### Spoiler gratificante asi es como quedara nuestro guardado de usuario!😎

````php
    public function save(User $user): void
    {
        $this->model::create($user->toPrimitives());
    }
````

<br>
<br>
<br>