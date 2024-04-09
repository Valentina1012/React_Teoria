## Renderizado y creación de elementos
Para renderizar html se necesita crear un "element", de esta forma:
<p><i>React.creatElement("button", null, "Me gusta")</i></p>
<p>Donde <b>"button"</b> es el elemento, <b>null</b> es el atributo o propiedad (si tuviera alguno se escribiría entre {} ) y <b>"Me gusta"</b> es lo que se envuelve dentro del elemento.<p><br>
<i>A tener en cuenta: React sólo renderiza 1 elemento</i> <br>
* React.fragment: Agrupa componentes para poder devolverlos renderizados

## Componentes
* Se utilizan para crear elementos
* Se escriben en Pascal case. Ej: RedButton. Es muy importante respetar esta regla porque sino
React no diferencia entre elementos hmtl y componentes
  
