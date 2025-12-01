# Branding Tokens - Starkline

Documentación de los tokens de diseño (colores, tipografías, estilos) del manual de marca de Starkline para implementación en el tema Dawn.

## 🎨 Paleta de Colores

### Colores Primarios
| Token CSS | Valor HEX | Uso |
|-----------|-----------|-----|
| `--starkline-primary` | `#000000` | Color principal de marca, botones CTA, enlaces |
| `--starkline-secondary` | `#FFFFFF` | Fondos, textos sobre primario |
| `--starkline-accent` | `#FF6B00` | Destacados, ofertas, badges |

### Colores de Estado
| Token CSS | Valor HEX | Uso |
|-----------|-----------|-----|
| `--starkline-success` | `#28A745` | Confirmaciones, stock disponible |
| `--starkline-warning` | `#FFC107` | Advertencias, últimas unidades |
| `--starkline-error` | `#DC3545` | Errores, validaciones fallidas |
| `--starkline-info` | `#17A2B8` | Información adicional, tooltips |

### Colores Neutros
| Token CSS | Valor HEX | Uso |
|-----------|-----------|-----|
| `--starkline-gray-100` | `#F8F9FA` | Fondos suaves, secciones alternas |
| `--starkline-gray-300` | `#DEE2E6` | Bordes, divisores |
| `--starkline-gray-700` | `#495057` | Textos secundarios |
| `--starkline-gray-900` | `#212529` | Textos principales |

## 🔤 Tipografías

### Familia de Fuentes
```css
--font-body-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
--font-heading-family: 'Poppins', 'Inter', sans-serif;
```

### Tamaños
| Token CSS | Valor | Uso |
|-----------|-------|-----|
| `--font-size-xs` | `0.75rem` (12px) | Etiquetas, badges |
| `--font-size-sm` | `0.875rem` (14px) | Textos secundarios |
| `--font-size-base` | `1rem` (16px) | Texto base |
| `--font-size-lg` | `1.125rem` (18px) | Destacados |
| `--font-size-xl` | `1.25rem` (20px) | Subtítulos |
| `--font-size-2xl` | `1.5rem` (24px) | Títulos H3 |
| `--font-size-3xl` | `2rem` (32px) | Títulos H2 |
| `--font-size-4xl` | `2.5rem` (40px) | Títulos H1 |

### Pesos
```css
--font-weight-normal: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
```

## 🔘 Componentes

### Botones
```css
/* Botón primario */
.btn-primary {
  background-color: var(--starkline-primary);
  color: var(--starkline-secondary);
  border-radius: 8px;
  padding: 12px 24px;
  font-weight: var(--font-weight-semibold);
  transition: all 0.2s ease;
}

.btn-primary:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
}
```

### Espaciado
| Token CSS | Valor | Uso |
|-----------|-------|-----|
| `--spacing-xs` | `4px` | Micro espacios |
| `--spacing-sm` | `8px` | Espacios pequeños |
| `--spacing-md` | `16px` | Espacios medios |
| `--spacing-lg` | `24px` | Espacios grandes |
| `--spacing-xl` | `32px` | Separación de secciones |
| `--spacing-2xl` | `48px` | Márgenes principales |

### Bordes y Sombras
```css
--border-radius-sm: 4px;
--border-radius-md: 8px;
--border-radius-lg: 12px;
--border-radius-full: 9999px;

--shadow-sm: 0 1px 2px rgba(0, 0, 0, 0.05);
--shadow-md: 0 4px 6px rgba(0, 0, 0, 0.1);
--shadow-lg: 0 10px 15px rgba(0, 0, 0, 0.1);
```

## 📱 Responsividad

### Breakpoints
```css
--breakpoint-sm: 640px;   /* Móvil grande */
--breakpoint-md: 768px;   /* Tablet */
--breakpoint-lg: 1024px;  /* Desktop */
--breakpoint-xl: 1280px;  /* Desktop grande */
```

## 🎯 Implementación

### Archivos a Modificar
1. **`assets/base.css`**: Variables CSS root
2. **`config/settings_schema.json`**: Exponer colores en editor
3. **`snippets/button.liquid`**: Aplicar estilos de botones
4. **`sections/*.liquid`**: Usar variables en secciones

### Ejemplo de Uso
```liquid
<button class="btn-primary" style="background-color: var(--starkline-primary)">
  Comprar Ahora
</button>
```

---

**Nota**: Estos son valores placeholder. Actualiza con los datos reales del manual de marca de Starkline antes de implementar en producción.
