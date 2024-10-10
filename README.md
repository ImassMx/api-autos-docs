# API Autos

> Version 1.0.0

## Path Table

| Method | Path | Description |
| --- | --- | --- |
| POST | [/oauth/token](#postoauthtoken) | OAuth2 Token |
| GET | [/api/catalog/forma-pago](#getapicatalogforma-pago) | Forma de Pago |
| GET | [/api/catalog/plazo/{producto}](#getapicatalogplazoproducto) | Plazo |
| GET | [/api/catalog/paquete/{producto}](#getapicatalogpaqueteproducto) | Paquete |
| GET | [/api/catalog/tipo-persona](#getapicatalogtipo-persona) | Tipo de Persona |
| GET | [/api/catalog/sucursal](#getapicatalogsucursal) | Sucursales |
| GET | [/api/catalog/sexo](#getapicatalogsexo) | Sexo |
| GET | [/api/catalog/tipo-valor](#getapicatalogtipo-valor) | Tipo Valor |
| GET | [/api/catalog/tipo-vehiculo](#getapicatalogtipo-vehiculo) | Tipo Vehículo |
| GET | [/api/catalog/tipo-seguro](#getapicatalogtipo-seguro) | Tipo Seguro |
| GET | [/api/catalog/modelo/auto/Particular](#getapicatalogmodeloautoparticular) | Modelo |
| GET | [/api/catalog/marca/auto/Particular](#getapicatalogmarcaautoparticular) | Marca |
| GET | [/api/catalog/producto](#getapicatalogproducto) | Producto |
| GET | [/api/catalog/submarca/auto/Particular](#getapicatalogsubmarcaautoparticular) | Submarca |
| GET | [/api/catalog/descripcion/auto/Particular](#getapicatalogdescripcionautoparticular) | Descripción |
| GET | [/api/catalog/cp](#getapicatalogcp) | CP |
| POST | [/api/cotizacion](#postapicotizacion) | Paso 1. Crear Cotización |
| GET | [/api/cotizacion/{id}](#getapicotizacionid) | Detalle Cotización |
| POST | [/api/cotizacion/{id}](#postapicotizacionid) | Paso 3. Elegir Aseguradora |
| PUT | [/api/cotizacion/{id}](#putapicotizacionid) | Paso 5. Actualizar Cotización |
| GET | [/api/cotizacion/{id}/Voluntario](#getapicotizacionidvoluntario) | Paso 2. Comparador Cotización |
| POST | [/api/asegurado](#postapiasegurado) | Paso 4. Crear Asegurado |
| POST | [/api/cotizacion/{id}/emitir](#postapicotizacionidemitir) | Paso 6. Emitir |
| GET | [/api/cotizacion/{id}/poliza](#getapicotizacionidpoliza) | Descarga Poliza |
| GET | [/api/cotizacion/{id}/recibo](#getapicotizacionidrecibo) | Descarga Recibos |

## Reference Table

| Name | Path | Description |
| --- | --- | --- |
| noauthAuth | [#/components/securitySchemes/noauthAuth](#componentssecurityschemesnoauthauth) |  |
| bearerAuth | [#/components/securitySchemes/bearerAuth](#componentssecurityschemesbearerauth) |  |

## Path Details

***

### [POST]/oauth/token

- Summary  
OAuth2 Token

- Security  
noauthAuth  

#### RequestBody

- multipart/form-data

```ts
{
  grant_type?: string
  client_id?: string
  client_secret?: string
  scope?: string
}
```

#### Responses

- 200 Successful response

`application/json`

***

### [GET]/api/catalog/forma-pago

- Summary  
Forma de Pago

#### Responses

- 200 Successful response

`application/json`

***

### [GET]/api/catalog/plazo/{producto}

- Summary  
Plazo

#### Responses

- 200 Successful response

`application/json`

***

### [GET]/api/catalog/paquete/{producto}

- Summary  
Paquete

#### Responses

- 200 Successful response

`application/json`

***

### [GET]/api/catalog/tipo-persona

- Summary  
Tipo de Persona

#### Responses

- 200 Successful response

`application/json`

***

### [GET]/api/catalog/sucursal

- Summary  
Sucursales

#### Responses

- 200 Successful response

`application/json`

***

### [GET]/api/catalog/sexo

- Summary  
Sexo

#### Responses

- 200 Successful response

`application/json`

***

### [GET]/api/catalog/tipo-valor

- Summary  
Tipo Valor

#### Responses

- 200 Successful response

`application/json`

***

### [GET]/api/catalog/tipo-vehiculo

- Summary  
Tipo Vehículo

#### Responses

- 200 Successful response

`application/json`

***

### [GET]/api/catalog/tipo-seguro

- Summary  
Tipo Seguro

#### Responses

- 200 Successful response

`application/json`

***

### [GET]/api/catalog/modelo/auto/Particular

- Summary  
Modelo

#### Responses

- 200 Successful response

`application/json`

***

### [GET]/api/catalog/marca/auto/Particular

- Summary  
Marca

#### Responses

- 200 Successful response

`application/json`

***

### [GET]/api/catalog/producto

- Summary  
Producto

#### Responses

- 200 Successful response

`application/json`

***

### [GET]/api/catalog/submarca/auto/Particular

- Summary  
Submarca

#### Parameters(Query)

```ts
marca?: string
```

#### Responses

- 200 Successful response

`application/json`

***

### [GET]/api/catalog/descripcion/auto/Particular

- Summary  
Descripción

#### Parameters(Query)

```ts
marca?: string
```

```ts
modelo?: integer
```

#### Headers

```ts
Accept?: string
```

#### Responses

- 200 Successful response

`application/json`

***

### [GET]/api/catalog/cp

- Summary  
CP

#### Parameters(Query)

```ts
cp?: integer
```

#### Headers

```ts
Accept?: string
```

#### Responses

- 200 Successful response

`application/json`

***

### [POST]/api/cotizacion

- Summary  
Paso 1. Crear Cotización

#### Headers

```ts
Content-Type?: string
```

```ts
Accept?: string
```

#### RequestBody

- application/json

```ts
{
}
```

#### Responses

- 200 Successful response

`application/json`

***

### [GET]/api/cotizacion/{id}

- Summary  
Detalle Cotización

#### Headers

```ts
Content-Type?: string
```

```ts
Accept?: string
```

#### Responses

- 200 Successful response

`application/json`

***

### [POST]/api/cotizacion/{id}

- Summary  
Paso 3. Elegir Aseguradora

#### Headers

```ts
Content-Type?: string
```

```ts
Accept?: string
```

#### RequestBody

- application/json

```ts
{
}
```

#### Responses

- 200 Successful response

`application/json`

***

### [PUT]/api/cotizacion/{id}

- Summary  
Paso 5. Actualizar Cotización

#### Headers

```ts
Content-Type?: string
```

```ts
Accept?: string
```

#### RequestBody

- application/json

```ts
{
}
```

#### Responses

- 200 Successful response

`application/json`

***

### [GET]/api/cotizacion/{id}/Voluntario

- Summary  
Paso 2. Comparador Cotización

#### Headers

```ts
Content-Type?: string
```

```ts
Accept?: string
```

#### Responses

- 200 Successful response

`application/json`

***

### [POST]/api/asegurado

- Summary  
Paso 4. Crear Asegurado

#### Headers

```ts
Content-Type?: string
```

```ts
Accept?: string
```

#### RequestBody

- application/json

```ts
{
}
```

#### Responses

- 200 Successful response

`application/json`

***

### [POST]/api/cotizacion/{id}/emitir

- Summary  
Paso 6. Emitir

#### Headers

```ts
Content-Type?: string
```

```ts
Accept?: string
```

#### RequestBody

#### Responses

- 200 Successful response

`application/json`

***

### [GET]/api/cotizacion/{id}/poliza

- Summary  
Descarga Poliza

#### Headers

```ts
Content-Type?: string
```

```ts
Accept?: string
```

#### Responses

- 200 Successful response

`application/json`

***

### [GET]/api/cotizacion/{id}/recibo

- Summary  
Descarga Recibos

#### Headers

```ts
Content-Type?: string
```

```ts
Accept?: string
```

#### Responses

- 200 Successful response

`application/json`

## References

### #/components/securitySchemes/noauthAuth

```ts
{
  "type": "http",
  "scheme": "noauth"
}
```

### #/components/securitySchemes/bearerAuth

```ts
{
  "type": "http",
  "scheme": "bearer"
}
```
