# Portafolios del grupo 4GS122

**Desarrollo de Software V (8400)** · II Semestre 2026
Prof. José Peralta B. · Universidad Tecnológica de Panamá, Centro Regional de Veraguas

Directorio del grupo: una sola página que enlaza el portafolio de cada
estudiante. Es la puerta de entrada al trabajo del semestre.

Publicado en:

```
https://joseperaltab-utp-fisc.github.io/2026ii-dsv-directorio-4gs122/
```

---

## Si eres estudiante

**Tu línea ya está creada**, con tu número y tu nombre. No la escribas de nuevo
ni la muevas de sitio: lo único que tienes que cambiar son **tus dos enlaces**.

### 1. Localiza tu ficha

En `docs/index.html`, busca tu código. Por ejemplo, el número 07:

```html
<article>
  <p class="codigo">4GS122-07</p>
  <h3>Nombre Apellido</h3>
  <ul class="enlaces">
    <li><a href="#">Página personal</a></li>
    <li><a href="#">Prácticas y laboratorios</a></li>
  </ul>
</article>
```

### 2. Cambia los dos `href`

Sustituye cada `#` por la dirección correspondiente de tu portafolio:

```html
    <li><a href="https://TU-USUARIO.github.io/TU-REPOSITORIO/">Página personal</a></li>
    <li><a href="https://TU-USUARIO.github.io/TU-REPOSITORIO/modulos/">Prácticas y laboratorios</a></li>
```

El primero lleva a tu página personal; el segundo, al índice de tus entregas.
**No toques nada más del archivo**, ni la ficha de ningún compañero.

### 3. Entrega el cambio

```bash
git switch -c 4gs122-07
git add docs/index.html
git commit -m "Agrega el portafolio de 4GS122-07"
git push -u origin 4gs122-07
```

Y abre un *pull request* desde GitHub.

### Por qué así

Si cada uno inserta su línea donde quiere, veinte personas editan la misma zona
del archivo y Git no puede fusionar sin conflictos. Con la lista ya creada, cada
quien modifica dos atributos de **su** línea y las fusiones son automáticas.

---

## Cómo se lee la página

| Elemento | Qué significa |
| --- | --- |
| Ficha con borde ámbar | El ejemplo resuelto: así debe quedar la tuya. |
| Enlaces con borde punteado | Esa entrada todavía apunta a `#`: sin publicar. |
| Enlace **Página personal** | La portada del portafolio del estudiante. |
| Enlace **Prácticas y laboratorios** | El índice de sus entregas por módulo. |
| Un enlace que da **404** | La dirección está puesta pero la página no existe. |

## Estructura

```
2026ii-dsv-directorio-4gs122/
├── README.md
├── .gitattributes          ← finales de línea LF: evita conflictos falsos
├── .gitignore
└── docs/                   ← lo que publica GitHub Pages
    ├── index.html          ← la lista del grupo
    └── assets/css/directorio.css
```
