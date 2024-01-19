# Temario - Caso de Uso: Crear Usuario

<img src="laravel-2.svg" alt="Laravel Logo" width="100" height="50">

### En este temario solo y unicamnte trabajaremos con el caso de uso de crear usuario!

###### Que??? Solo eso??? Si yo en 10 lineas de mi controlador puedo hacerlo!😀

###### Efectivamente solo sera ese caso de uso, con una pequena diferencia!

### 🚀<span style="color:blue">SOBRE-INGENERIA DE SOFWARE!</span>🚀

#### Spoiler final de como quedara nuestro controlador!

````php
final class CreateUserController extends BaseController
{
    public function __invoke(string $uuid, Request $request): JsonResponse
    {
        $this->dispatch(
            new CreateUserCommand(
                uuid    : $uuid,
                email   : $request->email,
                password: $request->password,
            )
        );

        response()->json(null, Response::HTTP_CREATED);
    }
}
````

## Temas a abordar
<img src="solid.png" alt="Laravel Logo" width="70%" height="70%">


