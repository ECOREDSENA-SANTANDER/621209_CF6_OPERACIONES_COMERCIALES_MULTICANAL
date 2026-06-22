<template lang="pug">
  .curso-main-container.pb-3
    BannerInterno(icono="far fa-question-circle" titulo="Actividad didáctica")
    .container.tarjeta.tarjeta--blanca.p-4.p-md-5
      // Para cuestionario usar: ActividadController(:cuestionario="cuestionario") 
      // Para parrafo usar: ActividadController(:parrafo="parrafo")
      ActividadController(:cuestionario="cuestionario")
  </template>

<script>
import ActividadController from '@ecored-sena/base-kit/plugin/components/actividad/ActividadController.vue'

export default {
  name: 'ActividadDidactica',
  components: {
    ActividadController,
  },
  data: () => ({
    cuestionario: {
      tema: 'Cuestionario: atención al cliente en el <i>retail.</i>',
      titulo: 'Cuestionario',
      introduccion:
        '<b> Objetivo:</b> verificar la comprensión de los conceptos fundamentales relacionados con la atención al cliente en el <i>retail</i>, el mercadeo <i>mix</i>, la clasificación de clientes, las técnicas de servicio, los protocolos organizacionales, la satisfacción del cliente, la trazabilidad del servicio y el trámite de PQRS. ',
      barajarPreguntas: true,
      titulo_aprobado: '¡BUEN TRABAJO!',
      titulo_reprobado: 'VUELVA A INTENTARLO',
      preguntas: [
        {
          id: 1,
          texto:
            'En el contexto del <i>retail</i>, una adecuada atención al cliente contribuye principalmente a:',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Reducir todos los canales de contacto.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Eliminar la necesidad de protocolos.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Favorecer la fidelización y el aumento de la clientela.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Reemplazar el conocimiento del producto.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 2,
          texto: 'Los componentes principales del mercadeo <i>mix</i> son:',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Producto, precio, plaza y promoción.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Cliente, factura, bodega y caja.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Venta, despacho, inventario y reporte.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Protocolo, encuesta, queja y reclamo.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 3,
          texto: 'La plaza, dentro del mercadeo <i>mix</i>, se relaciona con:',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'La cantidad de dinero que paga el cliente.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Los canales por los cuales el producto llega al consumidor.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'La formulación interna del producto.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Las normas de cortesía empresarial.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 4,
          texto: 'La omnicanalidad permite que el cliente:',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Use solo un canal físico de atención.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Reciba mensajes diferentes en cada canal.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Tenga una experiencia integrada y coherente en canales <i>online</i> y <i>offline</i>.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Evite todo contacto con la empresa.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 5,
          texto:
            'Si una persona aconseja a otra sobre qué producto comprar, cumple el papel de:',
          imagen: require('@/assets/actividad/imagen05.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Usuario.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Ejecutor.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Cliente agresivo.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Influyente.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 6,
          texto: 'Un cliente indeciso se caracteriza porque:',
          imagen: require('@/assets/actividad/imagen6.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Toma decisiones rápidas y declara sus intenciones.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Suele no tener claro lo que quiere y tarda en decidir.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Considera que todos deben estar a su servicio.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Rebate todos los argumentos con firmeza.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 7,
          texto: 'Ante un cliente discutidor, la actuación más adecuada es:',
          imagen: require('@/assets/actividad/imagen7.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Responder con cortesía, firmeza y argumentos claros.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Evitar escucharlo para reducir el tiempo de atención.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Atenderlo sin ofrecer explicaciones.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Prometer soluciones que no se pueden cumplir.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 8,
          texto: 'Segmentar a los clientes ayuda a la empresa a:',
          imagen: require('@/assets/actividad/imagen8.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Tratar a todos de forma idéntica sin analizar diferencias.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Eliminar las expectativas del servicio.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Reconocer necesidades, deseos y formas de trato diferentes.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Suspender la comunicación de <i>marketing</i>.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 9,
          texto: 'Los momentos de verdad son importantes porque:',
          imagen: require('@/assets/actividad/imagen9.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Solo ocurren después de la venta.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Permiten identificar experiencias del cliente frente al servicio recibido.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Eliminan la necesidad de escuchar al cliente.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Se limitan a trámites administrativos internos.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 10,
          texto:
            'Un plan de contingencia en servicio al cliente debe permitir:',
          imagen: require('@/assets/actividad/imagen10.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Planear cómo actuar y comunicar soluciones ante situaciones inesperadas.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Ocultar al cliente los problemas del servicio.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Evitar la coordinación entre colaboradores.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Suspender temporalmente la atención.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 11,
          texto: 'La comunicación asertiva se caracteriza por:',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Imponer una opinión sin escuchar al cliente.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Expresar necesidades con respeto, honestidad y claridad.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Usar reproches personales para persuadir.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Evitar toda argumentación.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 12,
          texto: 'Una técnica útil de comunicación asertiva en el trabajo es:',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Juzgar de inmediato la conducta del cliente.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Exigir antes de argumentar.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Escuchar activamente y hablar en primera persona.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Usar información hiriente para cerrar la conversación.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 13,
          texto: 'En el proceso de comunicación, el <i>feedback</i> permite:',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Confirmar que el mensaje fue recibido y comprendido.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Sustituir al emisor.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Eliminar las barreras comunicativas automáticamente.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Cambiar el código del mensaje sin acuerdo.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 14,
          texto: 'La comunicación no verbal incluye principalmente:',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Facturas, órdenes y fichas técnicas.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Gestos, contacto visual, postura y movimientos corporales.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Solo mensajes escritos.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Únicamente llamadas telefónicas.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 15,
          texto:
            'Al atender una llamada o requerimiento, una pauta adecuada es:',
          imagen: require('@/assets/actividad/imagen05.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Tomar decisiones precipitadas para terminar rápido.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Ignorar los protocolos de presentación y despedida.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Transmitir seguridad, mantener la calma y aplicar los protocolos.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Evitar preguntar por las necesidades del usuario.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 16,
          texto: 'El ciclo de servicio ayuda a la organización a:',
          imagen: require('@/assets/actividad/imagen6.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Pensar desde la experiencia del cliente y reconocer momentos de verdad.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Reducir la calidad del servicio a la despedida.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Suprimir la responsabilidad de directivos y colaboradores.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Atender solo las quejas formales.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 17,
          texto:
            'En el triángulo del servicio, el cliente debe entenderse como:',
          imagen: require('@/assets/actividad/imagen7.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Un elemento secundario frente a los sistemas.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'El eslabón más importante alrededor del cual giran estrategias y actores.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Un colaborador interno de la empresa.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'La herramienta técnica del proceso.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 18,
          texto: 'Un protocolo de atención al cliente es útil porque:',
          imagen: require('@/assets/actividad/imagen8.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Permite que cada colaborador actúe sin criterios comunes.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Elimina la necesidad de capacitar al personal.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Unifica conceptos y procedimientos para brindar una atención consistente.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Sustituye la cortesía por trámites internos.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 19,
          texto: 'La trazabilidad del servicio permite:',
          imagen: require('@/assets/actividad/imagen9.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Reconstruir la historia y recorrido de un producto o servicio.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Eliminar el monitoreo posventa.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Desconocer el origen de los componentes.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Evitar el registro de datos del proceso.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 20,
          texto:
            'Cuando un cliente presenta una recomendación o idea para mejorar el servicio, corresponde a una:',
          imagen: require('@/assets/actividad/imagen10.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Queja.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Petición.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Sugerencia.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Orden de compra.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
      ],
      mensaje_final_aprobado: 'Ha superado la actividad.',
      mensaje_final_reprobado:
        'Le recomendamos volver a revisar el componente formativo e intentar nuevamente la actividad didáctica. ',
    },
  }),
}
</script>
