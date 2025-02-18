name: Solicitud de Prestaciones
description: Solicita un servicio o soporte técnico del SIO-ICM.
title: "[Solicitud] Breve descripción del servicio requerido"
labels: ["solicitud", "pendiente revisión"]
assignees: ["usuario-asignado"]

body:
  - type: markdown
    attributes:
      value: |
        ## 🚢 Solicitud de Prestación de Servicios del SIO
        Por favor, completa el siguiente formulario para solicitar un servicio.

  - type: input
    id: nombre
    attributes:
      label: "Nombre del solicitante"
      placeholder: "Ejemplo: Juan Pérez"

  - type: input
    id: email
    attributes:
      label: "Correo Electrónico"
      placeholder: "ejemplo@empresa.com"

  - type: dropdown
    id: tipo_servicio
    attributes:
      label: "Tipo de servicio requerido"
      options:
        - Instrumentación Oceanográfica
        - Procesamiento de Datos
        - Asesoría Técnica
        - Otro (especificar en la descripción)

  - type: textarea
    id: descripcion
    attributes:
      label: "Descripción detallada"
      description: "Describe qué necesitas y cualquier información relevante."
      placeholder: "Ejemplo: Necesitamos calibrar un sensor de conductividad..."

  - type: checkboxes
    id: confirmacion
    attributes:
      label: "Confirmación"
      options:
        - label: "Confirmo que he revisado la documentación disponible antes de enviar esta solicitud."
