# Hooks
## useState()
useStatees un Hook de React que permite agregar una variable de estado a su componente.<br>
const [state, setState] = useState(initialState)
La convención es nombrar variables de estado como [something, setSomething] si se usara "array destructuring".<br>
* initialState: El valor que desea que tenga el estado inicialmente. Puede ser un valor de cualquier tipo, pero existe un comportamiento especial para las funciones. Este argumento se ignora después del renderizado inicial.
<p>useStatedevuelve una matriz con exactamente dos valores:</p>

* El estado actual. Durante el primer renderizado, coincidirá con el que initialStatehas pasado.
* La setfunción que le permite actualizar el estado a un valor diferente y activar una nueva representación.



## useEffect()
<p>useEffectes es un Hook, por lo que solo puedes llamarlo en el nivel superior de tu componente o en tus propios Hooks. No puedes llamarlo bucles internos o condiciones. Si lo necesita, extraiga un nuevo componente y mueva el estado a él. Si no estás intentando sincronizar con algún sistema externo,  probablemente no necesites un Effect.</p>
Debe pasar dos argumentos a useEffect:<br>
* <b>Setup:</b> Una función de configuración con código de configuración que se conecta a ese sistema. Cuando su componente se agregue al DOM, React ejecutará su función de configuración. Después de cada renderizado con dependencias modificadas, React primero ejecutará la función de limpieza (si la proporcionó) con los valores anteriores y luego ejecutará su función de configuración con los nuevos valores. <i>Debería devolver una función de limpieza con un código de limpieza que se desconecte de ese sistema.</i><br><br>
* <b>Dependencies(opcional):</b> Una lista de dependencias que incluye todos los valores de su componente utilizados dentro de esas funciones. Los valores reactivos incluyen accesorios, estado y todas las variables y funciones declaradas directamente dentro del cuerpo del componente. </p>
