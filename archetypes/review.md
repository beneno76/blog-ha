---
title: "{{ replace .File.ContentBaseName "-" " " | title }}"
date: {{ .Date }}
draft: true
summary: "Resumen de una línea: qué es y si vale la pena."
categorias: ["Sensores"]          # Sensores, Iluminación, Enchufes, Cámaras, Climatización...
etiquetas: ["Tuya"]
protocolos: ["Zigbee"]            # Zigbee, Wi-Fi, Bluetooth, Matter, Thread, RF 433...
cover:
  image: "portada.jpg"           # foto guardada en esta misma carpeta
  alt: "Foto del producto"
producto:
  nombre: "Nombre del producto"
  link: "https://es.aliexpress.com/item/XXXX.html"
  tienda: "AliExpress"
  precio: "US$ 0"
  fecha_compra: "2026-01"
  integracion: "ZHA / Zigbee2MQTT / Tuya / ESPHome / Local Tuya / MQTT"
  nota: 4                         # de 1 a 5
---

{{< ficha >}}

## Qué es

Qué compré, para qué lo quería y en qué parte de la casa lo uso.

## Unboxing y construcción

![Caja y contenido](caja.jpg)

Calidad, tamaño, materiales y lo que trae la caja.

![Placa por dentro](placa.jpg)

## Integración con Home Assistant

Pasos para emparejarlo y qué entidades aparecen.

![Dispositivo en Home Assistant](ha.png)

```yaml
# Automatización de ejemplo
alias: Ejemplo
triggers:
  - trigger: state
    entity_id: binary_sensor.ejemplo
    to: "on"
actions:
  - action: light.turn_on
    target:
      entity_id: light.ejemplo
```

## Uso en el día a día

Fiabilidad, alcance, batería y problemas encontrados.

## Pros y contras

**👍 Pros**
- 

**👎 Contras**
- 

## Veredicto

¿Lo volvería a comprar?
