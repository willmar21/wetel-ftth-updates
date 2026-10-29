# WETEL FTTH · actualizaciones

Este repositorio público distribuye únicamente la aplicación genérica y su interfaz compilada. No contiene proyectos de red, ubicaciones de usuarios, configuración privada de satélite ni llaves privadas. El código del producto se mantiene en su repositorio privado.

Instala la APK como actualización, sin desinstalar ni borrar datos. Después abre **Actualizaciones** en la aplicación Android. Cada paquete de interfaz se descarga completo, autentica con ECDSA y verifica por SHA256 antes de aplicarse. Se conserva la interfaz anterior para recuperación. Android siempre solicita confirmar la instalación de una APK.

`stable.json` es un sobre firmado: `payload` contiene JSON UTF-8 en Base64 y `signature` una firma ECDSA P-256 / SHA256 en DER. `public-key.spki.b64` contiene la llave pública de verificación. La app lleva esta llave incorporada; no la descarga de este repositorio para decidir confianza.

El servicio de actualización no sube proyectos ni credenciales del dispositivo. Necesita Internet para consultar/descargar; el diseño y la cartografía regional siguen locales. La resolución/licencia del satélite es independiente.

Los recursos de terceros conservan los avisos de licencia dentro de cada paquete. Canal piloto; la validación física en cada dispositivo se documenta por separado.
