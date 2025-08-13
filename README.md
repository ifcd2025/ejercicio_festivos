https://openholidaysapi.org/PublicHolidays?countryIsoCode=CODIGOISO&languageIsoCode=ES&validFrom=FECHAINICIAL&validTo=FECHAFINAL

Para mostrar las fechas en formato día-mes-año, podemos usar esta función, siendo fechaISO una cadena de texto con la fecha

 ```javascript
function formatearFecha(fechaISO) {
  const fecha = new Date(fechaISO);
  return fecha.toLocaleDateString('es-ES', {
    year: 'numeric',
    month: '2-digit',
    day: '2-digit'
  });
}
 ```
