# API de Operaciones de Cadenas

Esta API proporciona operaciones básicas de cadenas, incluyendo concatenación, substring y verificación de contenido.

## Endpoints

### Concatenación

- **URL:** `/concat`
- **Método:** `GET`
- **Parámetros de consulta:**
  - `str1`: La primera cadena para concatenar.
  - `str2`: La segunda cadena para concatenar.
- **Ejemplo de uso con curl:**

```bash
curl -X GET 'http://localhost:8080/concat?str1=hello&str2=world'
```

### Substring

- **URL:** `/substring`
- **Método:** `GET`
- **Parámetros de consulta:**
  - `str`: La cadena de la que obtener el substring.
  - `beginIndex`: El índice inicial del substring.
  - `endIndex`: El índice final del substring.
- **Ejemplo de uso con curl:**

```bash
curl -X GET 'http://localhost:8080/substring?str=helloworld&beginIndex=0&endIndex=5'
```

### Contains

- **URL:** `/contains`
- **Método:** `GET`
- **Parámetros de consulta:**
  - `str`: La cadena en la que buscar.
  - `substr`: La subcadena para buscar en `str`.
- **Ejemplo de uso con curl:**

```bash
curl -X GET 'http://localhost:8080/contains?str=helloworld&substr=world'
```

---
