<div align="center">

# ZIVLO

**Cobra en segundos. Sin internet. Sin complicaciones.**

</div>

---

## 👋 Bienvenido a ZIVLO

Somos una organización dedicada a desarrollar soluciones tecnológicas para el comercio latinoamericano real. Nuestro producto principal es un **punto de venta (POS) offline-first** que convierte cualquier smartphone Android en una caja registradora completa, sin necesidad de internet ni hardware costoso.

---

## 🎯 Nuestra Misión

> Eliminar las barreras tecnológicas para pequeños comerciantes en Latinoamérica, proporcionando herramientas accesibles que funcionen en las condiciones reales de conectividad de la región.

---

## 📦 Repositorios

| Repositorio | Descripción | Estado |
|-------------|-------------|--------|
| [**zivlo-app**](https://github.com/ZIVLO-Team/zivlo-app) | App móvil Flutter — POS offline-first | ✅ En desarrollo |
| [**zivlo-docs**](https://github.com/ZIVLO-Team/zivlo-docs) | Documentación oficial del proyecto | ✅ Disponible |
| [**zivlo-backend**](https://github.com/ZIVLO-Team/zivlo-backend) | API FastAPI + PostgreSQL para sincronización | 📋 Pendiente |
| [**zivlo-license-generator**](https://github.com/ZIVLO-Team/zivlo-license-generator) | Generador de licencias JWT | 📋 Pendiente |

---

## 🚀 Producto Principal: Zivlo POS

El punto de venta diseñado para el comercio real en Latinoamérica.

### Características Principales

| Feature | Descripción |
|---------|-------------|
| 📷 **Escaneo** | Código de barras con cámara (EAN, QR, Code128, UPC-A) |
| 🛒 **Carrito** | Gestión de compras con descuentos y totales automáticos |
| 💵 **Pagos** | Efectivo, tarjeta y pago mixto con calculadora de cambio |
| 🖨️ **Impresión** | Conecta impresoras térmicas Bluetooth 58mm/80mm |
| 📊 **Historial** | Consulta de ventas por fecha con resúmenes diarios |
| 📦 **Catálogo** | Gestión completa de productos con stock y categorías |
| 🚫 **Offline** | 100% funcional sin conexión a internet |

### ¿Para quién es Zivlo?

- 🏪 Tiendas de abarrotes y retail
- 🛒 Supermercados pequeños
- 🎪 Stands de exposición y ferias
- 🚚 Vendedores ambulantes
- 💼 Emprendedores en formación

---

## 🏗️ Arquitectura Técnica

Utilizamos **Clean/Hexagonal Architecture** para construir software escalable, testeable y mantenible.

```
┌─────────────────────────────────────────┐
│     Presentation Layer (Flutter)        │
│         BLoCs · Widgets · UI            │
├─────────────────────────────────────────┤
│      Application Layer                  │
│    Use Cases · Either<Failure, T>       │
├─────────────────────────────────────────┤
│         Domain Layer                    │
│  Entities · Value Objects · Ports       │
├─────────────────────────────────────────┤
│     Infrastructure Layer                │
│   Adapters · Hive · Hardware · API      │
└─────────────────────────────────────────┘
```

### Stack Tecnológico

| Capa | Tecnologías |
|------|-------------|
| **Mobile** | Flutter 3.x, Dart 3.x |
| **Estado** | BLoC Pattern (`flutter_bloc`) |
| **Backend** | FastAPI, PostgreSQL, SQLAlchemy |
| **Base de Datos** | Hive (local), PostgreSQL (server) |
| **Hardware** | `mobile_scanner`, `bluetooth_thermal` |
| **Licencias** | JWT con firma HMAC-SHA256 |

---

## 🎨 Identidad de Marca

### Nuestro Logo

El símbolo de Zivlo fusiona un **rayo** (velocidad, energía, instantáneo) con la silueta de un **recibo de papel** (borde dentado característico). La lectura es inmediata: velocidad + comercio.

<div align="center">

**Logo Principal**

<div style="display:inline-flex;align-items:center;gap:14px;">
  <svg width="52" height="72" viewBox="0 0 52 72" fill="none" xmlns="http://www.w3.org/2000/svg">
    <path d="M38 2 L14 36 H24 L6 70 H9 L13 63 L17 70 L21 63 L25 70 L29 63 L33 70 L37 63 L41 70 H44 L44 70 L28 36 H38 Z" fill="#E94560"/>
  </svg>
  <span style="font-family:'Syne',sans-serif;font-weight:800;font-size:56px;color:#ffffff;line-height:1;">zivlo</span>
</div>

**Símbolo (Ícono de App)**

<svg width="64" height="88" viewBox="0 0 52 72" fill="none" xmlns="http://www.w3.org/2000/svg" style="background:#1A1A2E;padding:16px;border-radius:16px;">
  <path d="M38 2 L14 36 H24 L6 70 H9 L13 63 L17 70 L21 63 L25 70 L29 63 L33 70 L37 63 L41 70 H44 L44 70 L28 36 H38 Z" fill="#E94560"/>
</svg>

</div>

### Paleta de Colores

<div align="center">

| Color | Hex | Uso |
|-------|-----|-----|
| <div style="width:80px;height:50px;background:#E94560;border-radius:8px;margin:8px auto;"></div> | `#E94560` | **Accent** — CTAs, logo, acciones principales |
| <div style="width:80px;height:50px;background:#1A1A2E;border-radius:8px;margin:8px auto;"></div> | `#1A1A2E` | **Primary** — Fondos, app icon |
| <div style="width:80px;height:50px;background:#0F3460;border-radius:8px;margin:8px auto;"></div> | `#0F3460` | **Surface** — Cards, sheets |
| <div style="width:80px;height:50px;background:#00D97E;border-radius:8px;margin:8px auto;"></div> | `#00D97E` | **Success** — Confirmaciones, stock |
| <div style="width:80px;height:50px;background:#FFB830;border-radius:8px;margin:8px auto;"></div> | `#FFB830` | **Warning** — Alertas, cambios |

</div>

### Tipografía

| Fuente | Uso | Peso |
|--------|-----|------|
| **Syne** | Display, Headlines | 700–800 |
| **DM Sans** | Body, UI, Botones | 300–600 |
| **Space Mono** | Números, Precios, Recibos | 400, 700 |

---

## 📊 Métricas de Éxito

| Meta | Objetivo |
|------|----------|
| ⏱️ Tiempo de transacción | < 20 segundos (escanear → cobrar → imprimir) |
| 🎯 Tasa de error en escaneo | < 2% |
| 🔗 Conexión BT | < 3 segundos |
| 💾 Pérdida de datos | 0% |
| 📈 Retención a 30 días | 70% |

---

## 🤝 Contribuir

¡Las contribuciones son bienvenidas! Revisa los repositorios individuales para guías específicas de contribución.

### Código de Conducta

- 🌟 Sé respetuoso y colaborativo
- 🎯 Enfócate en el impacto real para usuarios
- 📚 Comparte conocimiento abiertamente
- 🐛 Reporta bugs y sugiere mejoras

---

## 📄 Licencia

Todos los repositorios de ZIVLO-Team están licenciados bajo **MIT License** a menos que se indique lo contrario.

---

## 📞 Contacto

| Canal | Enlace |
|-------|--------|
| 🌐 Website | [zivlo.app](https://zivlo.app) (próximamente) |
| 📧 Email | contact@zivlo.app |
| 💬 Issues | [GitHub Issues](https://github.com/ZIVLO-Team/zivlo-app/issues) |
| 📦 Releases | [GitHub Releases](https://github.com/ZIVLO-Team/zivlo-app/releases) |

---

<div align="center">

### 🚀 Únete a nosotros

**Hecho con ❤️ para el comercio real en Latinoamérica**

[ZIVLO-Team](https://github.com/ZIVLO-Team) © 2024

</div>
