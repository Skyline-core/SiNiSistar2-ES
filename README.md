# SiNiSistar 2 — Pack de idioma Español (Mod)

Traducción no oficial al español con el sistema **Mod / Localize** del juego (v1.2.0+).  
Compatible con **SiNiSistar 2 v1.3.1**.

Licencia: [Creative Commons Atribución 4.0 Internacional (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

---

## Requisito: parche R18 (Steam)

En la versión Steam **LITE** / filtrada el juego **ignora los idiomas Mod**. Sin el parche, la carpeta puede estar bien puesta y aun así no aparece **Español**.

1. Descarga el parche oficial: https://erogejapan.com/patch/sinisistar2/  
   (PC, versión que coincida con tu juego, p. ej. 1.3.1)
2. Copia `SiNiSistar2_Data` y `Mod` del zip sobre la carpeta del juego.
3. Al arrancar debe **desaparecer LITE**.

Solo entonces el juego listará idiomas en `Mod\Localize\`.

---

## Instalación del pack (una sola carpeta)

Basta con **una** carpeta: `Español` (no hace falta también `Spanish`).

Colócala en la **raíz del juego** (junto a `SiNiSistar2.exe`):

```text
<carpeta del juego>\Mod\Localize\Español\
├── LocalizeTable.json
├── LocalizeTableChoice.json
├── LocalizeTableEvent.json
├── LocalizeTableNameText.json
└── TextSetting.json
```

Ejemplo Steam:

```text
G:\SteamLibrary\steamapps\common\SiNiSistar 2\Mod\Localize\Español\
```

Desde este repositorio, copia la carpeta `Mod` completa a la raíz del juego (o solo `Mod\Localize\Español`).

### AppData (opcional)

El juego también puede leer:

```text
%USERPROFILE%\AppData\LocalLow\Uu\SiNiSistar2\Mod\Localize\Español\
```

**No hace falta duplicar** el pack ahí si ya está en la carpeta del juego. Usa AppData solo si prefieres no tocar la instalación de Steam. Si dejas las dos, verás el idioma dos veces en la lista.

### Activar en el juego

1. Cierra el juego, instala el pack y (si aplica) el parche R18.
2. Arranca el juego.
3. **Ajustes → Language / Idioma**.
4. Avanza con ←/→ **después** de Japanese / English / 中文 / 한국어 hasta **Español**.
5. Sal del menú (Esc).

El nombre en la lista es el de la carpeta (`Español`).

---

## Contenido del pack

| Archivo | Qué traduce |
|---|---|
| `LocalizeTable.json` | Menús, objetos, estados, enemigos, misiones… |
| `LocalizeTableChoice.json` | Opciones de diálogo |
| `LocalizeTableEvent.json` | Diálogos / eventos |
| `LocalizeTableNameText.json` | Nombres en conversaciones |
| `TextSetting.json` | Fuente, tamaño y velocidad del texto |

### `TextSetting.json`

```json
{
    "OneCharWaitTime": 0.01,
    "WINDOWS_FontSetting": {
        "FontName": "Arial",
        "FontSize": 14
    },
    "MAC_FontSetting": {
        "FontName": "Helvetica",
        "FontSize": 14
    }
}
```

`FontName` debe existir en el sistema (con acentos: á, é, ñ, ¿, ¡).

---

## Si no aparece Español

| Causa | Qué hacer |
|---|---|
| Sigue saliendo **LITE** | Instala el [parche R18](https://erogejapan.com/patch/sinisistar2/) |
| Carpeta mal anidada | `Mod\Localize\Español\*.json` (no `Mod\Español\` ni doble subcarpeta) |
| Otra instalación | Copia junto al `.exe` que abre Steam |
| Dos entradas iguales | Borra el duplicado en AppData o en el juego; deja solo una carpeta `Español` |

---

## Desinstalación

Borra `Mod\Localize\Español` en la carpeta del juego y vuelve a un idioma oficial en ajustes.

---

## Notas

- Texto en texturas (logos, etc.) no se traduce con este sistema.
- HP / MP se dejan como en el original.
- Fan-made: puede haber frases por pulir.
- Este pack es una traducción de fan; el juego y sus derechos pertenecen a sus autores.

---

## Créditos

- Juego: **Uu** (ねんない / みーくん) — [Ci-en](https://ci-en.dlsite.com/creator/2462)
- Parche R18 Steam: [Eroge Japan](https://erogejapan.com/patch/sinisistar2/)
- Pack ES: comunidad / uso personal

## Licencia

El contenido original de este repositorio (traducción y documentación) se publica bajo [CC BY 4.0](LICENSE).  
SiNiSistar 2 y sus materiales oficiales © Uu / respectivos titulares.
