# Co-creacion de moneda

Con este sistema se pretende crear un protocolo de creación de tokens distribuido entre los usuarios de una misma comunidad, permitiendo que sea la propia comunidad de forma democrática la que decida cuándo y cuántos tokens tiene derecho a crear cada miembro de la comunidad y por tanto controlar la masa monetaria en todo momento.

El sistema consta de dos contratos inteligentes:

## A - Contrato DAO Censal (CDC). 

Consiste en un conjunto de contratos inteligentes de gestión y gobernanza conformando entre ellos una Organización Autónoma descentralizada de tipo membership o 1 usuario 1 token 1 voto

### El CDC contará con:
* Un token de gobernanza 1 usuario <-> 1 token
* Sistema de votación
* Capacidad de ejecución de contratos inteligentes externos previa votación. 

Este contrato o grupo de contratos no es necesario desarrollarlo puesto que ya hay desarrollos que podrían servir a este cliente, como Aragon Client Membership

## B - Contrato de distribución (CD). 

Consiste en un contrato ERC20 ampliado con una serie de particularidades y que gestionará la moneda común de los censados en CDC (poseedores de tokens).

Cualquier CC puede reclamar tokens de CD, MMCs, hasta un límite marcado desde CDC por votación de los CCCC durante un periodo máximo marcado por un bloque de la cadena determinado también por los CCCC.

El propietario del contrato será CDC y este podrá establecer tras votación de sus miembros:
* Cuántos tokens se pueden reclamar al mes por cada censado (MTT).
* Próximo bloque (PBR) en el que los usuarios podrán reclamar nuevas monedas.

## Sistema de reclamación de tokens

El sistema de reclamación de tokens por parte de los CCCC de forma individual, hace que, en caso de tener que pagar un GAS excesivo, sea compensado con la adquisición de los tokens reclamados, a la vez que descarga de un posible airdrop excesivamente costoso para quien tuviera que ejecutarlo.
Se entiende que los CCCC tratarán de crear una masa monetaria suficiente para operar en su economía pero no excesivamente grande como para convertir al token en moneda inflacionaria.

## Sin límites a la iniciativa ni a la propiedad privada

Como se observa, no se limita la cantidad máxima de MCC que puede acumular un mismo usuario, ya que de lo contrario se estaría limitando la iniciativa y el derecho fundamental a la propiedad privada.

Tampoco se le niega a nadie la reclamación de nuevas monedas en el periodo estipulado para ello, ya que algo así constituiría una discriminación.
