## LDAP

Es un protocolo que se usa de forma dubyacente en los servicios de directorio

**Protocolo Ligero de Acceso a Directorios**

Se manejan objetos, como por ejemplo un usuario. Agregando, eliminando o modificando entradas en notacion LDAP

`dn: CN=Miguel Gudino,OU=Sysadmin,DC=etermax,CD=com`

El formato de entrada LDAP básicamente tiene
dn = "nombre distinguido" un nombre de entrada único 
luego los atributos y valores asociados con esa entrada= 

- CN es el "nombre común" del objeto. En este caso, como es una persona, usamos "Miguel Gudino" 
- OU es la unidad organizativa, como un grupo. En este caso, se usa Sysadmin. 
- DC es el componente principal. Entonces, example.com está dividido en example y com. 

[Mas info](https://en.wikipedia.org/wiki/LDAP_Data_Interchange_Format)

## Servicios de directorio

Son bases de datos que se utilizan para refecenciar objetos dentro de una red, estos objetos pueden ser usuarios, grupos, dispositivos.

### Group Policy Object

Set de politicas (o directivas) y preferencias que son aplicadas a un grupo de objetos en un directorio

Las directivas son configuraciones que vuelven a aplicar cada pocos minutos y no se supone que sean modificadas ni siquiera por los admin locales. De manera predeterminada se reaplican cada 90 min

Las preferencias son como una plantilla predefinida pero que el usuario puede cambiar y se mantendra el cambio

muchas directivas y preferencias en las GPO se representan como valores en el registro de Windows

¿Cómo hacen las computadoras unidas a un dominio para obtener sus GPO? Cuando una computadora o un usuario unido a un dominio inicia sesión en el dominio por comunicación con un controlador de dominio, ese DC le brinda a la computadora una lista de directivas de grupo que debe aplicar. La computadora luego descarga esas directivas desde una carpeta especial llamada Sysvol, que se exporta como recurso compartido de red desde cada controlador de dominio. Esta carpeta se replica entre todos los controladores de dominio y también puede contener cosas como secuencias de comandos de inicio y cierre de sesión. Una vez que la computadora descargó sus GPO, los aplica.